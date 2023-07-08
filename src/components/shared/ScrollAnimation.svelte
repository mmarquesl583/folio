<div class="centralize">
  <div class="indicator"></div>
</div>

<style>
  .centralize {
    position: relative; /* Adicionar a propriedade position: relative; */
  }

  .indicator {
    width: 40px;
    height: 62px;
    border: 2px solid #fff;
    border-radius: 50px;
    position: absolute;
    opacity: 0;
    animation: fadeIn 1s ease-in-out forwards;
  }

  @keyframes fadeIn {
    0% {
      opacity: 0;
      top: 15px;
    }
    100% {
      opacity: 1;
      top: 15px;
    }
  }

  .indicator:before {
    content: "";
    position: absolute;
    width: 9px;
    height: 9px;
    background: #fff;
    margin: auto;
    left: 0;
    right: 0;
    border-radius: 50%;
    animation: animate 1s linear infinite;
  }

  @keyframes animate {
    0% {
      opacity: 1;
      top: 13px;
    }
    100% {
      opacity: 0;
      top: 45px;
      transform: scale(0.8);
    }
  }
</style>
