/* ==========================================================================
   MASTHEAD
   ========================================================================== */

.masthead {
  position: relative;
  border-bottom: 1px solid $border-color;
  -webkit-animation: $intro-transition;
  animation: $intro-transition;
  -webkit-animation-delay: 0.15s;
  animation-delay: 0.15s;
  z-index: 20;

  &__inner-wrap {
    @include clearfix;
    margin-left: auto;
    margin-right: auto;
    padding: 1em;
    max-width: 100%;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
    font-family: $sans-serif-narrow;

    @include breakpoint($x-large) {
      max-width: $max-width;
    }

    nav {
      z-index: 10;
    }

    a {
      text-decoration: none;
    }
  }
}

.site-logo img {
  max-height: 2rem;
}

.site-title {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -ms-flex-item-align: center;
  align-self: center;
  font-weight: bold;
  // z-index: 20;
}

.site-subtitle {
  display: block;
  font-size: $type-size-8;
}

.masthead__menu {
  float: left;
  margin-left: 0;
  margin-right: 0;
  width: 100%;
  clear: both;

  .site-nav {
    margin-left: 0;

    @include breakpoint($small) {
      float: right;
    }
  }

  ul {
    margin: 0;
    padding: 0;
    clear: both;
    list-style-type: none;
  }
}

.masthead__menu-item {
  display: block;
  list-style-type: none;
  white-space: nowrap;

  &--lg {
    padding-right: 2em;
    font-weight: 700;
  }
}
