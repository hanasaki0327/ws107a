<div class="content">
  <div style="width:50vw; margin-top:10vh">
  <form class="pure-form pure-form-aligned"> 
    <fieldset>
      <div class="pure-control-group">
        <label for="user">User</label>
        <input id="user" type="text" placeholder="User">
      </div>

      <div class="pure-control-group">
        <label for="password">Password</label>
        <input id="password" type="password" placeholder="Password">
      </div>

      <div class="pure-controls">
        <button type="button" class="pure-button pure-button-primary" onclick="login()">Login 登入</button>
      </div>
    </fieldset>
  </form>     
  </div>
</div>

<script>

function login() {
  var userBox = document.getElementById("user");
  var passwordBox = document.getElementById("password");
  ajaxPost("/login", {user:userBox.value, password:passwordBox.value});
}
</script>