<template>
    <div class="login-page-content">
        <div class="login-wrap">
            <div class="login-content">
                <div class="login-card">
                    <div class="login-logo mt-3">
                        <img src="../assets/logo.svg" class="img">
                    </div>
                    <div class="login-form">
                        <form @submit.stop.prevent="logIn" class="bs-component">
                            <div class="row">
                                <div class="col-xs-12">
                                    <fieldset class="form-group label-floating">
                                    <label class="control-label" for="email">E-mail</label>
                                    <input class="form-control" id="email" type="email" v-model="email" required />
                                    </fieldset>
                                </div>
                            </div>
                            <div class="row">
                                <div class="col-xs-12">
                                    <div class="form-group label-floating">
                                    <label class="control-label" for="password">Password</label>
                                    <input class="form-control" id="password" type="password" v-model="password" required />
                                    </div>
                                </div>
                            </div>
                            <br/>
                            <button class="au-btn au-btn--block m-b-20 small_font btn-primary text-center" type="submit">Entrar</button>
                            <div class="d-flex align-items-center py-3">
                                <span class="border-bottom w-100"></span>
                                <span class="mx-3">ou</span>
                                <span class="border-bottom w-100"></span>
                            </div>
                            <a href="" class="au-btn au-btn--block m-b-20 small_font btn-primary text-center">Cadastre-se</a>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'LoginForm',
  data () {
    return {
      buttonDescription: 'Entrar'
    }
  }
}
</script>

<style>
.login-page-content {
    background-color: #000271;
    background-size: 2000px 1250px;
    background-position: center;
    height: 100vh;
}

.login-wrap {
    max-width: 540px;
    padding-top: 8vh;
    margin: 0 auto;
}

.login-logo {
    text-align: center;
    margin-bottom: 30px;
}

.login-checkbox {
    display: -webkit-box;
    display: -webkit-flex;
    display: -moz-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: justify;
    -webkit-justify-content: space-between;
    -moz-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
}

.login-checkbox label input[type="checkbox"] {
    margin-right: 8px;
}

.login-checkbox > label > a {
    color: #ff2e44;
}

@media (max-width: 991px) {
    .login-checkbox {
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -webkit-flex-direction: column;
        -moz-box-orient: vertical;
        -moz-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
    }
}

.login-form .form-group label {
    display: block;
}

.login-content {
    background: #fff;
    padding: 30px 30px 20px;
    -webkit-border-radius: 2px;
    -moz-border-radius: 2px;
    border-radius: 2px;
}

.social-login-content {
    border-top: 1px solid #e7e7e7;
    border-bottom: 1px solid #e7e7e7;
     margin-top: 1rem!important;
}

/* ----- Buttons----- */
@media (max-width: 991px) {
    .au-btn {
        margin-top: 0;
    }
}
.au-btn {
    margin-top: 0;
    line-height: 45px;
    padding: 0 35px;
    text-transform: uppercase;
    color: #fff;
    -webkit-border-radius: 3px;
    -moz-border-radius: 3px;
    border-radius: 3px;
    -webkit-transition: all 0.3s ease;
    -o-transition: all 0.3s ease;
    -moz-transition: all 0.3s ease;
    transition: all 0.3s ease;
    cursor: pointer;
}

.au-btn:hover {
    color: #fff;
    background: #1A91FB;
}

.au-btn--blue2 {
    background: #00aced;
}

.au-btn--blue2:hover {
    background: #00a2e3;
}

.au-btn--block {
    display: block;
    width: 100%;
}

.au-btn-icon i {
    vertical-align: baseline;
    margin-right: 5px;
}

.au-btn--blue {
    background: #0486FB;
}

.au-btn--green {
    background: #63c76a;
}

.au-btn--gray-dark {
    background: #343a40;
}

.au-btn--green:hover {
    background: #59bd60;
}

.au-btn-plus {
    position: absolute;
    height: 45px;
    width: 45px;
    background: #63c76a;
    -webkit-border-radius: 100%;
    -moz-border-radius: 100%;
    border-radius: 100%;
    -webkit-transition: all 0.3s ease;
    -o-transition: all 0.3s ease;
    -moz-transition: all 0.3s ease;
    transition: all 0.3s ease;
    bottom: -22.5px;
    right: 45px;
    z-index: 3;
}

.au-btn-plus i {
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    -o-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    font-size: 15px;
    font-weight: 500;
    color: #fff;
}

.au-btn-plus:hover {
    background: #59bd60;
}

.au-btn-load {
    background: #808080;
    padding: 0 40px;
    font-size: 15px;
    color: #fff;
}

.au-btn-load:hover {
    background: #767676;
}

.au-btn-filter {
    font-size: 14px;
    color: #808080;
    background: #fff;
    -webkit-border-radius: 3px;
    -moz-border-radius: 3px;
    border-radius: 3px;
    -webkit-box-shadow: 0px 10px 20px 0px rgba(0, 0, 0, 0.03);
    -moz-box-shadow: 0px 10px 20px 0px rgba(0, 0, 0, 0.03);
    box-shadow: 0px 10px 20px 0px rgba(0, 0, 0, 0.03);
    padding: 0 15px;
    line-height: 40px;
    text-transform: capitalize;
}

.au-btn-filter i {
    margin-right: 5px;
}

.au-btn--small {
    padding: 0 20px;
    line-height: 40px;
    font-size: 14px;
}

.btn-blue {
    background: #018bff;
    border-color: #018bff;
}
.btn-blue:hover {
    background: #209aff;
    border-color: #209aff;
}

.page-wrapper2 {
    overflow: hidden;
    background: #e5e5e5;
    padding-bottom: 8vh;
}

.btn-primary {
    background: #0061b0;
    border-color: #0061b0;
}
.btn-primary:hover {
    background: #006bc2;
    border-color: #006bc2;
}

a {
    text-decoration: none;
}

.img {
    width: 180px;
    height: 90px;
}

</style>
