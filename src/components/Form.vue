<template>
  <form>
    <div class="form__details">
      <h1 class="form__title">
        A new way to <span class="form__title-highlight">stay productive!</span>
      </h1>
      <p class="form__subtitle">
        Find virtual study and co-working buddies to help get things done! Join
        the waitlist.
      </p>
    </div>

    <label class="form__input">
      <input type="email" class="form__input-field" placeholder="Enter your email address..." />
      <Button :title="'Notify Me'" :size="'medium'" />
    </label>
  </form>
</template>

<script>
import Button from "@/components/Button.vue";

export default {
  name: "form",
  components: {
    Button,
  },
  data() {
    return {
      email: "",
    };
  },
  methods: {
    setEmail: function (email) {
      this.email = email;
    },
  },
};
</script>

<style lang="scss" scoped>
form {
  width: 100%;
  
}

.form__details {

  @media screen and (max-width: 755px) {
    padding: 0 10%;
  }

   @media screen and (max-width: 600px) {
     padding: 0;
   }

  .form__title {
    font-size: 3.75rem;
    font-weight: normal;
    margin: 0;
    line-height: 1;

    @media screen and (max-width: 500px) {
      font-size: 2.75rem;
    }
  }

  .form__title-highlight {
    color: var(--col-primary);
    font-family: "Darker Grotesque", sans-serif;
  }
}

.form__input {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 45%;
  border-radius: 4px;
  border: 1px solid rgba(158, 158, 158, 0.514);
  margin: 2rem auto;
  padding: 0.3rem 0.3rem 0.3rem 1rem;

  @media screen and (max-width: 1000px) {
    width: 60%;
  }

  @media screen and (max-width: 755px) {
    width: 80%;
  }

  @media screen and (max-width: 600px) {
    width: 100%;
  }

  &:focus-within {
    border-color: var(--col-primary);
  }

  &-field {
    border: none;
    flex-grow: 1;
    outline: none;

    @media screen and (max-width: 365px) {
      overflow: hidden;
    }
    
    ::placeholder {
      color: var(--col-secondary-grey);
    }
  }
}
</style>
