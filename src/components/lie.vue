<template>
  <body style="height: 100%; font-family: 'Microsoft JhengHei UI' ;color: #666">
  <form method="post" id = "form1" style="height: 100%;">
    <div class = "dialog" style="height: 240px">
      <table style="width: 100%">
        <tbody>
        <tr>
          <td colspan="2">
            <h4 class="dialog-title">逢甲大學 NID 登入</h4>
          </td>
        </tr>
        <tr>
          <td style="padding-bottom: 3px;">
            <input name="ct" type="text" id="TextBox_nid" tabindex="1" class ="form-control" placeholder="NID">
          </td>
          <td rowspan="2" style="text-align: center;vertical-align: middle">
            <input type="submit" name="Button1" value="登入" id = "Button1" tabindex="3" class="btn btn-default" style="width: 70px;height: 70px">
          </td>
        </tr>
        <tr>
          <td>
            <input name="TextBox_pwd" type="password" id = "TextBox_pwd" tabindex="2" class="form-control" placeholder="Password">
          </td>
        </tr>
        <tr>
          <td style="padding: 5px;">
            <span id = "Label_msg" style="color: red;font-size: medium;">&nbsp;</span>
          </td>
        </tr>
        <tr>
          <td colspan="2" style="text-align: right">
            " 本系統採用NID驗證&nbsp;&nbsp;
            <img src="1.gif" width="50" alt="">
            <br>
            <a tabindex="1" onclick="goNIDa()" target="_blank">NID authentication</a>
          </td>
        </tr>
        </tbody>
      </table>
    </div>
    <div style="width:100%;height:100%;position: absolute;overflow:hidden;background-color:black">
      <div style="background-image:url('2.jpg');background-repeat:no-repeat;background-size:cover;background-position:center center;width:110%;height:110%;top:-5%;left:-5%;position:absolute;opacity:.6;" class="blur"></div>
    </div>
  </form>
  </body>
</template>

<script>

  function goNIDa() {
    window.open("https://netid.fcu.edu.tw/", "_blank").focus();
  }

</script>

<style scoped>
h4{
  font-size: 18px;
  margin-top: 10px;
  margin-bottom: 10px;
}

.form-control{
  box-sizing:border-box;
}
.dialog{
  margin: -115px 0 0 -180px;
  left: 50%;
  top: 40%;
  width: 360px;
  height: 230px;
  position: absolute;
  background-color: white;
  z-index: 10000;
  border-radius: 3px;
  padding:20px 30px 20px 30px;
  box-sizing: border-box;
  box-shadow: 0 2px 26px rgba(0, 0, 0, .5), 0 0 0 1px rgba(0, 0, 0, .1);
}
.dialog-title {
  font-weight: bold;
  line-height: 1.5em;
  color: #777;
}
.btn {
  display: inline-block;
  padding: 4px 10px;
  margin-bottom: 0;
  font-size: 14px;
  font-weight: 200;
  line-height: 1.42857143;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 4px;
}
input[type=submit]{
  -webkit-appearance: button;
  cursor: pointer;
}

.btn-default{
  color: #333333;
  background-color: #ffffff;
  border-color: #cccccc;
}


table{
  border-collapse: collapse;
  display: table;
  text-indent: initial;
}

.form-control{
  display: block;
  width: 100%;
  height: 34px;
  padding: 6px 12px;
  font-size: 14px;
  line-height: 1.42857143;
  color: #555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 4px;
}


.blur{
  filter: blur(10px);
}
body{
  font-size: 14px;
  line-height: 1.42857143;
  background-color: #ffffff;
  margin: 0;
  display: block;
}
div{
  display: block;
}

form{
  display: block;
  margin-top: 0;
}

a{
  color: #337ab7;
  text-decoration: none;
  background-color: transparent;
  cursor: pointer;
}
</style>