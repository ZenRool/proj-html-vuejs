<template>
  <form action="#">
    <input type="text" placeholder="Name*" required />
    <input type="email" placeholder="Emeil*" required />
    <input type="text" placeholder="Phone Number" />
    <input type="date" placeholder="Appointment Date" />
    <textarea placeholder="How can we help?*" required></textarea>
    <button>Make an appointment</button>
  </form>
</template>
<script>
export default {
  name: "FormAppointment",
};
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
form {
  input,
  textarea {
    background-color: transparent;
    color: white;
    border: 1px solid rgba($color: white, $alpha: 0.7);
    margin-bottom: 1.5rem;
    padding: 0.5rem;
    &::placeholder {
      color: rgba($color: white, $alpha: 0.7);
    }
  }
  input {
    height: 2.5rem;
    vertical-align: 1.5rem;
    width: 48%;
  }
  textarea {
    width: 100%;
    height: 100px;
  }
  button {
    width: 100%;
    height: 50px;
    color: white;
    background-color: $pelorous-vibrant;
    text-transform: uppercase;
    font-size: 1.2rem;
    border: none;
    cursor: pointer;
    &:hover {
      background-color: $pelorous;
    }
  }
}
</style>
