<template>
  <div>
    <h1>Please fill out our from...</h1>
    <form action="">
      <div id="form-header">
        <slot name='form-heade'></slot>
      </div>
      <div id="form-fields">
        <slot name='form-fields'></slot>

      </div>
      <div id="form-controls">
        <slot name='form-controls'></slot>

      </div>
      <div id="useful-links">
        <ul>
          <li><a href="#">Link 1</a></li>
          <li><a href="#">Link 2</a></li>
          <li><a href="#">Link 3</a></li>
          <li><a href="#">Link 4</a></li>
        </ul>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {};
  },
};
</script>

<style scoped>
div {
  max-width: 600px;
  margin: 20px auto;
  background: white;
  border-radius: 12px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

h1 {
  text-align: center;
  background: #3b82f6;
  color: white;
  padding: 20px;
  margin: 0;
  font-size: 1.6rem;
}

form {
  padding: 19px;
}


input, textarea, select {
  width: 91%;
  padding: 10px 16px;
  margin-bottom: 15px;
  border: 2px solid #e5e7eb;
  border-radius: 8px;
  font-size: 1rem;
  transition: all 0.3s;
}

input:focus, textarea:focus, select:focus {
  outline: none;
  border-color: #3b82f6;
  box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.15);
}


input::placeholder, textarea::placeholder {
  color: #9ca3af;
  opacity: 1;
}


button {
  background: #3b82f6;
  color: white;
  padding: 14px 25px;
  border: none;
  border-radius: 8px;
  font-size: 1.1rem;
  cursor: pointer;
  width: 100%;
  margin-top: 10px;
}

button:hover {
  background: #2563eb;
}


#useful-links {
  margin-top: 30px;
  padding-top: 20px;
  border-top: 1px solid #eee;
  text-align: center;
}

#useful-links ul {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

#useful-links a {
  color: #555;
  text-decoration: none;
}

#useful-links a:hover {
  color: #3b82f6;
}
</style>