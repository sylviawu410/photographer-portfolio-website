<template>
  <div class="home">
    <div class="section1">
      <div class="section1-left">
        <div class="section1-left-text">Stunning Photography by</div>
        <h1 class="section1-heading">Damien Braun</h1>
      </div>
      <svg class="section1-middle" xmlns="http://www.w3.org/2000/svg" width="262" height="256" viewBox="0 0 262 256"
        fill="none">
        <path
          d="M131 128.5C202.906 128.5 261.23 186.657 261.499 258.5H246.779C246.51 194.787 194.777 143.22 131 143.22C67.2232 143.22 15.4904 194.787 15.2211 258.5H0.500938C0.770414 186.657 59.0935 128.5 131 128.5ZM0.500938 -2.5H15.2211C15.4904 61.2136 67.2232 112.78 131 112.78C194.777 112.78 246.51 61.2136 246.779 -2.5H261.499C261.23 69.3432 202.906 127.5 131 127.5C59.0935 127.5 0.770412 69.3432 0.500938 -2.5ZM131 96.06C76.4575 96.06 32.2105 51.9792 31.9412 -2.5H46.6614C46.9305 43.8496 84.5871 81.34 131 81.34C177.413 81.34 215.069 43.8496 215.339 -2.5H230.059C229.79 51.9792 185.543 96.06 131 96.06ZM131 64.62C93.8213 64.62 63.6506 34.6153 63.3818 -2.5H78.1023C78.3707 26.4856 101.951 49.9 131 49.9C160.049 49.9 183.629 26.4856 183.898 -2.5H198.618C198.349 34.6153 168.179 64.62 131 64.62ZM131 159.94C185.543 159.94 229.79 204.02 230.059 258.5H215.339C215.069 212.151 177.413 174.66 131 174.66C84.5871 174.66 46.9305 212.151 46.6614 258.5H31.9412C32.2105 204.02 76.4575 159.94 131 159.94ZM131 191.38C168.179 191.38 198.349 221.384 198.618 258.5H183.898C183.629 229.515 160.048 206.1 131 206.1C101.951 206.1 78.3707 229.515 78.1023 258.5H63.3818C63.6506 221.384 93.8213 191.38 131 191.38Z"
          fill="#0E0E10" stroke="#1C1C21" />
      </svg>

      <div class="section1-right">
        <div class="section1-right-wrapper">
          <h1>Let’s</h1>
          <div class="purple-btn">
            <div class="purple-btn-background"></div>
            <svg class="purple-btn-svg" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
              fill="none">
              <path fill-rule="evenodd" clip-rule="evenodd"
                d="M8.25 3.75L19.5 3.75C19.6989 3.75 19.8897 3.82902 20.0303 3.96967C20.171 4.11032 20.25 4.30109 20.25 4.5V15.75C20.25 16.1642 19.9142 16.5 19.5 16.5C19.0858 16.5 18.75 16.1642 18.75 15.75V6.31066L5.03033 20.0303C4.73744 20.3232 4.26256 20.3232 3.96967 20.0303C3.67678 19.7374 3.67678 19.2626 3.96967 18.9697L17.6893 5.25L8.25 5.25C7.83579 5.25 7.5 4.91421 7.5 4.5C7.5 4.08579 7.83579 3.75 8.25 3.75Z"
                fill="white" />
            </svg>
          </div>
        </div>
        <h1>Work Together</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style>
@media screen and (min-width: 992px) {
  .home {
    /* margin-top: 300px; */
    margin-bottom: 200px;

  }

  .home .section1 {
    display: flex;
    padding: 0 80px;
    justify-content: space-between;
    align-items: center;
    height: 262px;
  }

  .home .section1-left {
    align-items: center;
  }

  .home .section1-left-text {
    color: var(--Grey-50, #797C86);
    font-size: 16px;
    font-weight: 600;
    line-height: normal;
    font-style: normal;
  }

  .home .section1-heading {
    font-size: 60px;
  }

  .hone .section1-right {
    display: flex;
  }

  .home .section1-right-wrapper {
    display: flex;
  }

  .home .purple-btn {
    float: inline-start;
    clear: none;
    margin-left: 12px;
    margin-top: 5px;
    position: relative;
    width: 104px;
    height: 56px;
    top: 0;
    left: 0;
  }

  .home .purple-btn-background {
    display: flex;
    padding: 28px 50px;
    align-items: center;
    gap: 10px;
    border-radius: 100px;
    background: var(--Purple-55, #4A2CED);
    box-shadow: 4px 4px 17.4px 0px rgba(255, 255, 255, 0.28) inset;
    position: relative;
    top: 0;
    left: 0;
  }

  .home .purple-btn-svg {
    position: absolute;
    top: 16px;
    left: 40px;
  }
}
</style>