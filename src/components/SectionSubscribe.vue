<template>
  <section id="subscribe" class="d-flex align-items-center">

    <!-- alert -->
    <div class="layover" v-if="alertActive">
      <div class="alert">
        <h2>
          La tua email è stata inviata con successo
          <i class="fa-solid fa-check"></i>
        </h2>
      </div>
    </div>

    <div class="container">
      <div class="row">
        <div class="col-12">
          <!-- card-subscribe -->
          <div class="card-subscribe text-white d-flex align-items-center">
            <div class="text-subscribe px-5">
              <h2>We Offer Awesome Services</h2>
              <p>
                When, while the lovely valley teems with vapour around meand the
                meridian sun strikes the upper surface.
              </p>
            </div>
            <div class="input-subscribe">           
                <input
                  type="email"
                  v-model.trim="term"
                  @keyup.enter="uploadMail"
                  placeholder="Enter Your Mail Address"
                  required
                />
                <button type="button" class="bg-blue" @click="uploadMail">
                  Subscribe
                </button>             
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionSubscribe",
  data() {
    return {
      term: "",
       alertActive: false,
    };
  },
  methods: {


     uploadMail() {
      //CONTROLLO//
      const lowerTerm = this.term.toLowerCase();
      if(!lowerTerm) return;

      //CONTROLLO//
        if (!lowerTerm.includes("@")) {
        return alert("inserisci email valida");
      }

      this.alertActive = true;
      setTimeout(() => {
        this.alertActive = false;
        this.term = '';
      }, 3000);
    }, 
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

/* alert */
 .layover {
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgba(0, 0, 0, 0.411);

  .alert {
    width: 680px;
    height: 80px;
    border-radius: 20px;
    box-shadow: 0 0 15px 0 black;
    border: 2px solid white;
    background: linear-gradient(
      270deg,
      rgba(2, 0, 36, 1) 0%,
      rgba(36, 36, 115, 1) 0%,
      rgba(0, 160, 186, 1) 100%
    );
    color: $bg-white;
  }
} 

#subscribe {
  height: 400px;
  background-image: linear-gradient(
    to bottom,
    $bg-lightwhite 50%,
    $bg-blue 50%
  );

  .card-subscribe {
    height: 260px;
    border-radius: 30px;
    background: rgb(0, 29, 36);
    background: linear-gradient(
      90deg,
      rgba(0, 29, 36, 1) 0%,
      rgba(100, 133, 145, 1) 0%,
      rgba(227, 18, 47, 1) 100%
    );

    .text-subscribe {
      width: 70%;
    }

    h2 {
      font-size: 3rem;
      font-weight: 700;
    }

    .input-subscribe {
      width: 365px;
      text-align: end;
      background-color: $bg-white;
      border-radius: 25px;
      padding: 5px;
      input {
        width: 250px;
        outline: none;
        border: 0;
      }
      button {
        border-radius: 25px;
        padding: 10px;
        border: none;
        &.bg-blue {
          background: linear-gradient(
            270deg,
            rgba(2, 0, 36, 1) 0%,
            rgba(36, 36, 115, 1) 0%,
            rgba(0, 160, 186, 1) 100%
          );
          color: $bg-white;
        }
        &.bg-blue:active {
          background: linear-gradient(
            90deg,
            rgba(0, 29, 36, 1) 0%,
            rgba(100, 133, 145, 1) 0%,
            rgba(227, 18, 47, 1) 100%
          );
          color: white;
        }
      }
    }
  }
}
</style>