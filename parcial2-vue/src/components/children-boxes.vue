<template>
  <section>
    <h2>Boxes</h2>
    <div class="boxes-layout">
      <aside class="profile-sidebar">
        <img
          src="../assets/roman.png"
          alt="Foto de perfil"
          class="foto-perfil"
        />
        <h3>Gersson Andrey Valencia Silva</h3>
        <p>Información breve sobre el usuario.</p>
      </aside>

      <div class="boxes-content">
        <p>Esta es la sección de "Boxes". El contenido iría aquí.</p>
        <div class="box">
          <h3>Box 1</h3>
          <p>Contenido personalizado del usuario.</p>
        </div>
        <div class="box">
          <h3>Box 2</h3>
          <p>Otra categoría o interés destacado.</p>
        </div>
        <div class="box">
          <h3>Box 3</h3>
          <p>Información adicional o widget.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ChildrenBoxes",
};
</script>

<style scoped>
.boxes-layout {
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 30px;
}

.profile-sidebar {
  background-color: white;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
  text-align: center;
}

.foto-perfil {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 10px;
}

.boxes-content {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.box {
  background-color: white;
  padding: 15px;
  border-radius: 6px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
}
</style>

    