<template>
  <div class="w-50">
      <form>
              <div class="input-group mb-3 w-100">
      <input
      v-model="form.title"
        type="text"
        class="form-control form-control-lg"
        aria-describedby="button-addon2"
      />
      <button
        class="btn btn-success"
        type="submit"
        id="button-addon2"
      >
        Add This to your list
      </button>
    </div>
      </form>

  </div>
</template>

<script>
export default {
  data() {
    return {
        form: new Form({
            title: '',
        })
    };
  },
  mounted() {
    console.log("Component mounted.");
  },
};
</script>
