<template>
  <header>
      <div class="container">
        <div class="ms_navbar d-flex align-items-center justify-content-between">

          <div class="ms_logo">
            <img src="../assets/img/dark-logo.png" alt="">
          </div>

          <div class="ms_navbar-right">
            <span class="ms_navbar-option">
              Home
              <i class="fas fa-chevron-down"></i>
            </span>
            <span class="ms_navbar-option">
              Pages
              <i class="fas fa-chevron-down"></i>
            </span>
            <span class="ms_navbar-option">
              Courses
              <i class="fas fa-chevron-down"></i>
            </span>
            <span class="ms_navbar-option">
              Features
              <i class="fas fa-chevron-down"></i>
            </span>
            <span class="ms_navbar-option">
              Blog
              <i class="fas fa-chevron-down"></i>
            </span>
            <span class="ms_navbar-option">
              Shop
              <i class="fas fa-chevron-down"></i>
            </span>
            <i class="far fa-user-circle ms_fa-user-circle"></i>
            <span class="ms_searchbar">
              <form id="form" role="search">
                <input type="search" id="query" placeholder="Search...">
                <button>
                  <i class="fas fa-search ms_search"></i>
                </button>
              </form>
            </span>
          </div>

          
        </div>
      </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>


<style scoped lang="scss">
@import '../assets/style/variables.scss';

header{
  box-shadow: 0px 3px 10px $color11;

  .container{
    

    .ms_navbar{
      height: 100px;

      .ms_logo{
        width: 150px;

        img{
          width: 100%;
          height: 100%;
        }
      }

      .ms_navbar-right{
        .ms_navbar-option{
          margin: 0 20px;

        }
        .ms_searchbar{
          display: inline-block;
        }
      }
    }
  }
}

.fa-chevron-down{
  width: 8px;
  vertical-align: middle;
  margin: 1px;
}
.ms_fa-user-circle{
  margin-right: 20px;
  vertical-align: middle;
}




form {
  background-color: $color11;
  width: 200px;
  height: 44px;
  border-radius: 5px;
  display: flex;
  flex-direction: row;
  align-items: center;
}
input {
  all: unset;
  font: 16px system-ui;
  color: #fff;
  height: 100%;
  width: 100%;
  padding: 6px 10px;
}
button {
  all: unset;
  cursor: pointer;
  width: 44px;
  height: 44px;
}
.ms_search{
  color: $color3;
  fill: currentColor;
  width: 15px;
  height: 24px;
  padding: 10px;
}

</style>
