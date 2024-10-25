<template lang="">
  <div id="member">
    <h2>Welceom member</h2>
    <div class="register">
      <div class="container">
        <form method="POST" action="#">
          <h3 class="text-center">Login</h3>
          <input
            type="text"
            class="form-control mt-2"
            maxlength="10"
            name="username"
            placeholder="username"
            required
          />
          <input
            type="password"
            class="form-control mt-2"
            maxlength="10"
            name="password"
            placeholder="password"
            required
          />
          <button
            type="submit"
            class="btn btn-primary form-control mt-3"
            name="submit"
          >
            Login
          </button>
        </form>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "member",
};
</script>


