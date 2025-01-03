
<template>
    <div class="container-fuild">

      <!--Background-->
      <div class="carousel-inner">
        <div>
          <div class="hero">
            <div class="bg-primary">
              <h1>
                Selamat Datang di Sekolah Pusat Keunggulan SMKN 4 Tasikmalaya
              </h1>
            </div>
          </div>
        </div>
      </div>
  
      <!--Sambutan-->
      <div class="container">
        <div class="row">
          <div class="clearfix">
            <div class="col-lg-4"></div>
            <img
              src="/assets/kepsek.jpg"
              class="col-md-6 float-md-end mb-3 ms-md-3 pt-5"
              alt="..."
              style="width: 25rem"
            />
            <h1 class="mt-5 text-center">Sambutan Kepala Sekolah</h1>
  
            <p class="pt-5">
              Assalamualaikum Warahmatullahi Wabarakatuh Selamat datang di SMKN 4
              Tasikmalaya. Segala puji dan syukur kita panjatkan kehadirat Allah
              SWT, semoga kita semua ada dalam lindungan-Nya. Dan atas
              perkenan-Nya pula kami dapat menghadirkan website SMK Negeri 4
              Tasikmalaya ini. Kami berharap dengan adanya website di SMK Negeri 4
              Tasikmalaya ini para pengunjung dapat mengenal lebih jauh tentang
              sekolah kami sehingga dapat mempererat tali silaturrahmi antara
              sekolah dengan masyarakat demi kemajuan kita bersama. Tiada gading
              yang tak retak, website kami ini masih dalam proses pengembangan,
              masih banyak kekurangan yang harus kami perbaiki. Kritik dan
              sarannya yang membangun sangat kami harapkan untuk pengembangan ke
              depan. Akhirnya, saya mengucapkan terimakasih yang sebesar-besarnya
              kepada semua pihak yang tidak dapat disebutkan satu segala bantuan
              dan persatu atas fasilitasnya yang telah diberikan semoga semua yang
              kita lakukan bermanfaat bagi masyarakat. Wassalamu'alaikum
              Warahmatullahi Wabarakatuh.
            </p>
          </div>
        </div>
      </div>
  
      <!--Statistik-->
      <div class="container">
        <h1 class="fs-1 text-center">Data Statistik</h1>
        <div class="row my-5 ms-5 text-white">
          <div class="col-lg-3">
            <div class="card bg-primary" style="height: 10rem">
              <div class="card-body">
                <h4 class="card-title text-md-center mt-5 fw-bold">
                  1500 jumlah siswa
                </h4>
              </div>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="card bg-primary" style="height: 10rem">
              <div class="card-body">
                <h4 class="card-title text-md-center mt-5 fw-bold">
                  18 Ekstrakurikuler
                </h4>
              </div>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="card bg-primary" style="height: 10rem">
              <div class="card-body">
                <h4 class="card-title text-md-center mt-5 fw-bold">
                  80 jumlah guru
                </h4>
              </div>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="card bg-primary" style="height: 10rem">
              <div class="card-body">
                <h4 class="card-title text-md-center mt-5 fw-bold">
                  10 jumlah administrasi
                </h4>
              </div>
            </div>
          </div>
        </div>
      </div>
  
      <!--Berita-->
      <div class="container">
        <h1 class="text-center mb-5">Berita Terkini</h1>
        <div class="row justify-content-center">
          <div
            v-for="(berita, i) in cover"
            :key="i"
            class="col-lg-4 d-flex justify-content-center"
          >
            <div class="card" style="width: 18rem">
              <img :src="berita.poto" class="card-img-top" alt="berita" />
              <div class="card-body">
                <h5 class="card-title">
                  {{ berita.judul }}
                </h5>
                <p class="card-text">
                  {{ berita.nama }}
                </p>
                <a
                  href="https://radartasik.disway.id/read/643944/pt-dam-jalin-kerjasama-dengan-smkn-4-tasikmalaya-terapkan-kurikulum-teknik-dan-bisnis-sepeda-motor-honda"
                  class="btn btn-primary"
                  >Lihat Selengkapnya</a
                >
              </div>
            </div>
          </div>
        </div>
      </div>
  
      <!--Jurusan-->
      <div class="container">
        <h1 class="text-center mb-5">Kompetensi Keahlian</h1>
        <div class="row">
          <div class="d-flex justify-content-center">
            <div class="col-lg-4">
              <div class="card mb-3">
                <div class="row g-0">
                  <div class="col-md-4">
                    <img
                      src="assets/pplg.jpeg"
                      class="img-fluid rounded-start"
                      alt="..."
                    />
                  </div>
                  <div class="col-md-8">
                    <div class="card-body">
                      <h5 class="card-title">
                        Pengembangan Perangkat Lunak & Gim (PPLG)
                      </h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="d-flex justify-content-center">
            <div class="col-lg-4">
              <div class="card mb-3">
                <div class="row g-0">
                  <div class="col-md-4">
                    <img
                      src="/assets/tjkt.jpeg"
                      class="img-fluid rounded-start"
                      alt="..."
                    />
                  </div>
                  <div class="col-md-8">
                    <div class="card-body">
                      <h5 class="card-title">
                        Teknik Jaringan Komputer & Telekomunikasi (TJKT)
                      </h5>
                    </div>
                  </div>
                </div>
              </div>
              <div class="card mb-3">
                <div class="row g-0">
                  <div class="col-md-4">
                    <img
                      src="/assets/tbsm.jpg"
                      class="img-fluid rounded-start"
                      alt="..."
                    />
                  </div>
                  <div class="col-md-8">
                    <div class="card-body">
                      <h5 class="card-title">
                        Teknik & Bisnis Sepeda Motor (TBSM)
                      </h5>
                    </div>
                  </div>
                </div>
              </div>
              <div class="card mb-3">
                <div class="row g-0">
                  <div class="col-md-4">
                    <img
                      src="/assets/dkv.jpeg"
                      class="img-fluid rounded-start"
                      alt="..."
                    />
                  </div>
                  <div class="col-md-8">
                    <div class="card-body">
                      <h5 class="card-title">Desain Komunikasi Visual (DKV)</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="d-flex justify-content-center">
            <div class="col-lg-4">
              <div class="card mb-3">
                <div class="row g-0">
                  <div class="col-md-4">
                    <img
                      src="/assets/toi.jpeg"
                      class="img-fluid rounded-start"
                      alt="..."
                    />
                  </div>
                  <div class="col-md-8">
                    <div class="card-body">
                      <h5 class="card-title">Teknik Otomasi Industri (TOI)</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .hero {
    background-image: url("/assets/v4tas.jpg");
    height: 100vh;
    width: 100vw;
    background-size: cover;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
  }
  </style>
  
  <script setup>
   useHead({
    title: "Beranda Page",
    meta: [
      {
        name: "description",
        content: "Beranda Page",
      },
    ],
  });
  const supabase = useSupabaseClient();
  
  const cover = ref([]);
  
  const getData = async () => {
    const { data, error } = await supabase.from("berita").select(`*`);
    if (data) cover.value = data;
  };
  
  onMounted(() => {
    getData();
  });
  </script>
  