<template>
  <div class="footer">
    <div class="container">
      <p>&copy; Beryl Thyer Memorial Africa Trust. Registered Charity Number 1112603.</p>
      <div class="footer__social">
        <a class="footer__link" href="https://twitter.com/btmat">twitter</a>
        <a class="footer__link" href="https://www.facebook.com/Beryl-Thyer-Memorial-Africa-Trust-168568809870673/">facebook</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss">
@import "./assets/styles/utilities/variables";

.footer {
  font-family: $f-sans;
  font-size: 1rem;
  padding: 50px 0;
  border-top: 1px solid $c-keyline;
  color: $c-grey;
  background: $c-white;
}

.footer__social {
  margin-top: 1em;
}

.footer__link {
  text-decoration: none;
  color: $c-green;
  margin-right: 1em;
  position: relative;

  &:after {
    position: absolute;
    content: '';
    height: 2px;
    bottom: 0;
    left: 0;
    width: 0;
    background: $c-green;
    transition: width $ease;
  }

  &:hover,
  &:focus {
    &:after {
      width: 100%;
    }
  }
}
</style>
