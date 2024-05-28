<template>
  <div class="home-page">
    <div class="page-header">
      <iframe
        width="1280"
        height="720"
        src="https://www.youtube-nocookie.com/embed/02G3GUt6Nzo?rel=0&amp;showinfo=0"
        frameborder="0"
        style="width: 1280px; height: 720px; margin-top: 60px;"
      >
      </iframe>
    </div>
    <div class="where-to-buy">
      <button>Where to buy?</button>
    </div>
    <div class="what-is-dead-cells">
      <section-title title="What is Dead Cells?"/>
      <div class="section">
        <p>
          Dead Cells is a rogue-lite, Castlevania-inspired action-platformer, allowing you to explore a sprawling, ever-changing castle… assuming you’re able to fight your way past its keepers.
        </p>
        <p>
          To beat the game, you’ll have to master 2D "souls-lite combat" with the ever-present threat of permadeath looming. No checkpoints. Kill, die, learn, repeat.
        </p>
        <ul>
          <li>
            <strong>RogueVania:</strong> Intense 2D action with the adrenaline pumping threat of permadeath in a castle full of cuddly creatures.
          </li>
          <li>
            <strong>Nonlinear progression:</strong> Unlock new levels with every death, take a new path. Tired of the stinking sewers? Why not take the ramparts?
          </li>
          <li>
            <strong>Souls-lite combat:</strong> Pattern-based bosses and minions, weapons and spells with unique gameplay. Roll roll roll your boat gently down the stream...
          </li>
          <li>
            <strong>Exploration:</strong> Secret rooms, hidden passages, charming landscapes. A fine place for a holiday.
          </li>
        </ul>
        <div class="section-videos">
          <video autobuffer="autobuffer" autoplay="autoplay" loop="loop" muted="muted" poster="https://dead-cells.com/img/roofPreview.jpg">
            <source src="https://dead-cells.com/video/roof.mp4" type="video/mp4">
            <source src="https://dead-cells.com/video/roof.webm" type="video/webm">
          </video>
          <video autobuffer="autobuffer" autoplay="autoplay" loop="loop" muted="muted" poster="https://dead-cells.com/img/bossFightPreview.jpg">
            <source src="https://dead-cells.com/video/bossFight.mp4" type="video/mp4">
            <source src="https://dead-cells.com/video/bossFight.webm" type="video/webm">
          </video>
        </div>
      </div>
    </div>
    <div class="on-android">
      <section-title title="Dead Cells on Android"/>
      <p>Get an alert when Dead Cells available on Android:</p>
    </div>
  </div>
</template>

<script>
import SectionTitle from '@/components/UI/SectionTitle.vue'

export default {
  components: { SectionTitle }

}
</script>

<style lang="scss" scoped>
.home-page {
  background-image: url("../assets/images/Background.png");
  min-height: 100vh;
  background-repeat: no-repeat;
  margin-top: 60px;

  .page-header {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 45px;

    iframe {
      box-shadow: 0 0 16px rgba(0,0,0,0.75);
    }
  }

  .where-to-buy {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 30px;

    button {
      width: 350px;
      background: linear-gradient(to bottom, #d1394e 50%, #cd2f46 50%);
      height: 90px;
      font-size: 60px;
      line-height: 90px;
      margin: 0 20px;
      border: none;
      border-bottom: 8px solid #832154;
      font-family: ATCKrueger, sans-serif;
      color: #FFF;
    }
  }

  .what-is-dead-cells {
    margin-bottom: 2%;
    .section {
      width: 740px;
      margin: 0 auto;
      padding: 20px;
      font-size: 1.1em;

      p {
        margin-bottom: 20px;
        font-size: 1.1em;
      }

      ul {
        column-count: 2;
        margin-bottom: 16px;
        margin-top: 10px;
        list-style: none;

        li {
          margin-bottom: 12px;
          font-size: 1.1em;

          strong {
            color: #A40239;
          }
        }
      }

      .section-videos {
        display: flex;
        justify-content: space-between;

        video {
          max-width: calc(50% - 10px);
          cursor: zoom-in;
          box-shadow: 0 0 16px rgba(0, 0, 0, 0.75);

        }
      }
    }
  }
}
</style>