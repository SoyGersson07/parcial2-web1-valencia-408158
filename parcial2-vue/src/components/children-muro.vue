<template>
  <section>
    <h2>Muro</h2>

    <div class="post-box">
      <textarea placeholder="¿Qué estás pensando?"></textarea>
      <div class="post-actions">
        <button>Adjuntar</button>
        <button>Publicar</button>
      </div>
    </div>

    <article class="post">
      <div class="post-header">
        <img
          src="../assets/jona.png"
          alt="Avatar Jonathan"
          class="post-avatar"
        />
        <div>
          <h3>Jonathan</h3>
          <p class="post-date">Hace 2 horas</p>
        </div>
      </div>
      <div class="post-content">
        <p>¡Hoy logré crear una SPA con JavaScript puro!!</p>
      </div>
      <div class="post-buttons">
        <button>Me gusta</button>
        <button>Comentar</button>
        <button>Compartir</button>
      </div>
    </article>

    <article class="post">
      <div class="post-header">
        <img src="../assets/images.jpeg" alt="Avatar Maria" class="post-avatar" />
        <div>
          <h3>Maria</h3>
          <p class="post-date">Hace 5 horas</p>
        </div>
      </div>
      <div class="post-content">
        <p>¿Alguien tiene recomendaciones de cursos de diseño UX? 🎨</p>
      </div>
      <div class="post-buttons">
        <button>Me gusta</button>
        <button>Comentar</button>
        <button>Compartir</button>
      </div>
    </article>
  </section>
</template>

<script>
export default {
  name: "ChildrenMuro",
};
</script>

<style scoped>
.post-box {
  background-color: white;
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
  margin-bottom: 20px;
}

.post-box textarea {
  width: 100%;
  padding: 10px;
  border-radius: 6px;
  border: 1px solid #ccc;
  resize: none;
}

.post-actions {
  margin-top: 10px;
  display: flex;
  gap: 10px;
}

button {
  background-color: #4267B2;
  color: white;
  border: none;
  padding: 8px 12px;
  border-radius: 4px;
  cursor: pointer;
}

.post {
  background-color: white;
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
  margin-bottom: 20px;
}

.post-header {
  display: flex;
  align-items: center;
  gap: 10px;
}

.post-avatar {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  object-fit: cover;
}

.post-date {
  font-size: 0.9em;
  color: #666;
  margin: 0;
}

.post-content {
  margin: 10px 0;
}

.post-buttons {
  display: flex;
  gap: 10px;
}
</style>

