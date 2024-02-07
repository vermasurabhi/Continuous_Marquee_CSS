# Continuous_Marquee_CSS
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>

.marquee {
  --gap: 0.5px;
  display: flex;
  position: relative;
  overflow: hidden;
  user-select: none;
  gap: var(--gap);
}

.marquee__content {
  flex-shrink: 0;
  display: flex;
  justify-content: space-around;
  gap: var(--gap);
  min-width: 100%;
  animation: scroll 20s linear infinite;
  font-size: 20px;
}

.marquee_reverse {
  animation-direction: reverse;
}

.marquee:hover .marquee_pause {
  animation-play-state: paused;
}


@keyframes scroll {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}
</style>
</head>
<body>
  <hr/><div style="text-align: center;">CONTINIOUS MARQUEE</div><hr/>
  <div class="marquee">
    <div class="marquee__content">
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    </div>

    <div aria-hidden="true" class="marquee__content">
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
      <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    </div>
  </div>
<hr/>
<div style="text-align: center;">REVERSE</div><hr/>
<div class="marquee">
  <div class="marquee_reverse marquee__content">
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
  </div>

  <div aria-hidden="true" class="marquee_reverse marquee__content">
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
  </div>
</div>
<hr/><div style="text-align: center;">PAUSE</div><hr/>
<div class="marquee">
  <div class="marquee_reverse marquee__content marquee_pause">
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
  </div>

  <div aria-hidden="true" class="marquee_reverse marquee__content marquee_pause">
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
    <div>THIS  IS  A  CONTINIOUS  MARQUEE   ✦</div>
  </div>
</div>
<hr/>

</body>
</html>
