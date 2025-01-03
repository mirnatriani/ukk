
<template>
    <div class="container pb-5">
      <h2 class="text-center pt-3">Ekstrakurikuler</h2>
      <div class="row flex justify-content-center">
        <div v-for="(eskul, i) in cover" :key="i" class="col-lg-3">
          <div class="card mb-5" style="width: 18rem">
            <img :src="eskul.poto" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">{{ eskul.nama }}</h5>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  useHead({
    title: "Ekstrakurikuler Page",
    meta: [
      {
        name: "description",
        content: "Ekstrakurikuler Page",
      },
    ],
  });
  const supabase = useSupabaseClient();
  
  const cover = ref([]);
  
  const getCover = async () => {
    const { data } = await supabase.from("eskul").select("*");
    if (data) cover.value = data;
  };
  
  onMounted(() => {
    getCover();
  });
  </script> 
  