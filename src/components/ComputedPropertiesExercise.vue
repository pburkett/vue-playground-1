<template>
  <div class="computed-properties-exercise container">
    <div class="row">
      <div class="col-12">
        <div class="border p-1">
          <div class="reverse-message">
            <p>Original Message: {{state.message}}</p>
            <p>Computed Reversed Message: {{state.reversedMessage}}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import { computed, reactive } from "vue";
export default {
  name: "computed-properties-exercise",
  setup() {
    const state = reactive({
<<<<<<< HEAD
=======
      // After getting this to work, challenge yourself to add an input field and bind message to it, so as you type the messag gets reversed!
>>>>>>> ea2854e813b8c2c107f2a92fea949d6ed6e3ccaf
      message: "Hello World!",
      reversedMessage: computed(() => {
        let out = ''
        for (let ind in state.message){
          out = state.message[ind] + out
        }
        return out
      }),
    });
    return {
      state,
    };
  },
};
</script>


<style scoped>
</style>
