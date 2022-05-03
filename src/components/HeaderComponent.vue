<template>
    <header>
      <div class="container">
        <div class="row jc-space-between">
          <div class="col">
            <div class="logo">
              <img src="@/assets/img/dc-logo.png" alt="">
            </div>
          </div>
          <div class="col">
            <nav>
              <ul>
                <li>characters</li>
                <li class="active">comics</li>
                <li>movies</li>
                <li>tv</li>
                <li>games</li>
                <li>collectibles</li>
                <li>videos</li>
                <li>fans</li>
                <li>news</li>
                <li>shop</li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderComponent'
}
</script>

<style lang="scss" scoped>
    header {

        .logo {
            display: flex;
            align-items: center;
            height: 100%;
        }

        nav {
            display: flex;
            align-items: center;
            height: 100%;

            ul {
                display: flex;
                list-style: none;
                height: 100%;


                li {
                    display: flex;
                    align-items: center;
                    text-transform: uppercase;
                    padding: 4rem 0;
                    margin: 0 1rem;
                    height: 100%;
                    border-bottom: 4px solid transparent;

                    &.active {
                        color: blue;
                        border-color: blue;
                    }

                }
            }
        }
    }
</style>