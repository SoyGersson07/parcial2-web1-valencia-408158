<template>
  <section>
    <h2>Información Personal</h2>
    <ul>
      <li>Email: gersson@example.com</li>
      <li>Teléfono: +57 300 123 4567</li>
      <li>Intereses: Programación, videojuegos, diseño</li>
      <li>Situación sentimental: Soltero</li>
    </ul>
    <div class="post-actions">
      <button>Me gusta</button>
      <button>Compartir</button>
    </div>
  </section>
</template>

<script>
export default {
  name: "ChildrenInfo",
};
</script>

<style scoped>
section {
  background-color: white;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
}

ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

li {
  margin-bottom: 8px;
}

.post-actions {
  margin-top: 15px;
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
</style>

