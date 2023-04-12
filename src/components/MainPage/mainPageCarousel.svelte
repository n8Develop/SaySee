<div class="container">
  <div class="left">
    <div class="leftItems">Left Arrow</div>
  </div>

  <div class="middle">
    <div class="middleItems">Carousel Placeholder</div>
  </div>

  <div class="right">
    <div class="rightItems">Right Arrow</div>
  </div>
</div>

<style>
  .container {
    grid-template-columns: 20%[left] 60% [middle] 20% [right];
    grid-template-areas: "left middle right";
    display: grid;
  }

  .left {
    background-color: rgb(197, 63, 161, 0.4);
    grid-column-start: left;
  }
  .leftItems {
    justify-self: center;
  }
  .middle {
    background-color: rgb(17, 163, 161, 0.4);
    grid-column-start: middle;
  }
  .middleItems {
    justify-self: center;
  }
  .right {
    background-color: rgb(97, 63, 61, 0.4);
    grid-column-start: right;
  }
  .rightItems {
    justify-self: center;
  }
</style>
