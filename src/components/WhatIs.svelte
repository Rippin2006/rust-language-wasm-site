<script>
  import textEditor from '../assets/text-editor.png';
  import terminal from '../assets/hacker.png';
  import browser from '../assets/browser.png';
  import devTools from '../assets/settings.png';
  let a = '커리큘럼';
</script>

<div class="whatIsSvelte-wrapper">
  <h3>{a}</h3>

  <div class="divp">
    <div class="left-icons">
      <div class="editor-div">
        <img class="editor-img" src={textEditor} alt="Code editor" />
        <h2>개발</h2>
        <p>개발을 중시합니다</p>
      </div>
      <div class="terminal-div">
        <img class="terminal" src={terminal} alt="Terminal" />
        <h2>해킹</h2>
        <p>해킹을 중시합니다</p>
      </div>
    </div>
    <div class="right-icons">
      <div class="browser-div">
        <img class="browser" src={browser} alt="Broswer View" />
        <h2>test1</h2>
        <p>test</p>
      </div>
      <div class="devTools-div">
        <img class="devTools" src={devTools} alt="devtools" />
        <h2>test2</h2>
        <p>test</p>
      </div>
    </div>
  </div>
</div>

<style>
  .whatIsSvelte-wrapper {
    background-color: white;
    text-align: center;
    height: calc(130vh - 180px);
  }

  h3 {
    margin: 0;
    padding: 40px 0 0 0;
    font-weight: 350;
    font-size: 500%;
    margin-bottom: 15px;
    color:black;
  }

  p {
    margin: 0;
    padding: 20px 0 40px 0;
    font-size: 130%;
    line-height: 135%;
  }

  .divp {
    display: flex;
    flex-wrap: wrap;
  }

  div.divp > div {
    flex: 20%;
    padding: 20px;
  }

  div.divp > div > div > img {
    height: 100px;
    width: auto;
  }

  @media screen and (max-width: 650px) {
    div.divp > div {
      flex: 50%;
    }
  }

  @media screen and (max-width: 600px) {
    .divp {
      flex-direction: column;
    }
  }
  @media screen and (max-width: 475px) {
    h3 {
      font-size: 200%;
    }
    p {
      font-size: 75%;
    }
  }
</style>


