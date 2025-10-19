<template>
  <section>
    <h2>Fotos</h2>
    <div class="photos-grid">
      <div class="photo-item">
        <img src="../assets/foto1.jpeg" alt="Foto 1" />
        <p>Fotografía</p>
      </div>
      <div class="photo-item">
        <img src="../assets/foto2.jpeg" alt="Foto 2" />
        <p>Cartagena</p>
      </div>
      <div class="photo-item">
        <img src="../assets/foto3.webp" alt="Foto 3" />
        <p>Gato</p>
      </div>
      <div class="photo-item">
        <img src="../assets/foto4.jpeg" alt="Foto 4" />
        <p>Cascada</p>
      </div>
      <div class="photo-item">
        <img src="../assets/foto5.jpg" alt="Foto 5" />
        <p>Luna</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ChildrenPhotos",
};
</script>

<style scoped>
.photos-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
  gap: 15px;
}

.photo-item {
  text-align: center;
  background-color: white;
  padding: 10px;
  border-radius: 6px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
}

.photo-item img {
  width: 100%;
  border-radius: 4px;
  margin-bottom: 5px;
}
</style>
