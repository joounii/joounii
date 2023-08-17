<body>
  <style>
    body, .jumbotron { padding: 30px; }
    .text-giant      { font-size: 40px; }
    .btn-crazy       {
      position: absolute;
      top: 30px;
      left: 35%;
      width: 30%;
      transition: 0.1s ease all;
      text-align: center;
    }
  </style>
  <button type="button" class="btn-crazy btn btn-lg btn-danger" onmouseenter="goCrazy.call(this)">
    Click Me!
  </button>
  <button type="button" class="btn-crazy btn btn-lg btn-primary" onmouseenter="goCrazy.call(this)">
    Click Me!
  </button>
  <button type="button" class="btn-crazy btn btn-lg btn-success" onmouseenter="goCrazy.call(this)">
    Click Me!
  </button>
  
  <script>
    function goCrazy() {
      const offsetLeft = Math.random() * (window.innerWidth - this.clientWidth);
      const offsetTop  = Math.random() * (window.innerHeight - this.clientHeight);
  
      console.log(offsetLeft, offsetTop);
  
      this.style.top = offsetTop + 'px';
      this.style.left = offsetLeft + 'px';
    }
  </script>
</body>
</html>
