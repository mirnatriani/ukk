<template>
    <div class="container pb-5">
      <h2 class="text-center pt-3">GALERI</h2>
      <div class="row flex justify-content-center">
        <div v-for="(galeri, i) in galeri" :key="i" class="col-lg-3">
          <div class="card mb-5" style="width: 18rem">
            <img :src="galeri.poto" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">{{ galeri.nama }} </h5>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>

<script setup>
useHead({
  title: "Galeri Page",
  meta: [
    {
      name: "description",
      content: "Galeri Page",
    },
  ],
});
const supabase = useSupabaseClient();

const galeri = ref([]);

const getData = async () => {
  const { data } = await supabase.from("galeri").select("*");
  if (data) galeri.value = data;
};

onMounted(() => {
  getData();
});
</script> 