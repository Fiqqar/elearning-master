<template>

    <body>
        <div class="wrapper">
            <form action="" class="register-container">
                <h2 class="title">Register</h2>
                <div class="input-container">
                    <input id="input-register" type="" name="name" placeholder="Username">
                </div>
                <div class="input-container">
                    <input type="date" name="birthdate" id="birth" required>
                </div>
                <div class="input-container">
                    <input id="input-register" type="password" name="pw" placeholder="Password">
                </div>
                <p id="login1">Already have an account?</p> <router-link to="/login" id="login">Login Here</router-link>
                <button class="registerbtn">Register</button>
            </form>
        </div>
    </body>
</template>

<script>
export default {
    name: 'SignupForm',
    data() {
        return {
        }
    },
    methods: {
        handleLogin() {
            console.log('Register button clicked');
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body {
    height: 100vh;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    /* Horizontally center */
    align-items: center;
    /* Vertically center */
    font-family: Arial, sans-serif;
    background: linear-gradient(to top, #a8e6cf, #fff9b1);
    background-size: cover;
}

.wrapper {
    width: 100%;
    max-width: 400px;
    /* Limit the form width */
    padding: 20px;
    background-color: #91c2ed;
    border-radius: 8px;
    box-shadow: 0 30px 8px rgba(0, 0, 0, 0.1);
}

.title {
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
}

.input-container {
    margin: 10px 0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding-right: 0px;
    margin-right: px;
    margin-left: px;
}

.input-container input {
    width: 100%;
    padding: 10px 1px;
    font-size: 16px;
    border: 1px solid #ddd;
    border-radius: 5px;
    outline: none;
    transition: border-color 0.3s, box-shadow 0.3s;
}

.input-container input:focus {
    border-color: #4a90e2;
    box-shadow: 0 0 10px rgba(49, 97, 151, 0.5);
}

.input-container label {
    font-size: 14px;
    margin-bottom: 5px;
    color: #555;
}


#input-register {
    border-radius: 1px;
    margin-left: 5px;
}

.registerbtn {
    width: 100%;
    padding: 12px 0px;
    font-size: 16px;
    font-weight: bold;
    color: white;
    background-color: #4a90e2;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    text-transform: uppercase;
    transition: background-color 0.3s, transform 0.25s;
    position: relative;
    transition: transform 0.1s ease-in-out;
}

.registerbtn:hover {
    background-color: #357ab8;
    transform: scale(0.95);
}

.registerbtn:active {
    transform: scale(0.90);
}

.registerbtn:focus {
    outline: 2px solid #6cb3ff;
    outline-offset: 2px;
}

#login {
    color: white;
    text-decoration: underline;
    font-size: 14px;
    display: inline-block;
    transition: color 0.3s ease-in-out;
    margin-bottom: 10px;
}

#login:hover {
    color: #357ab8;
}

#login1 {
    color: white;
    text-decoration: none;
    font-size: 14px;
    margin-top: 10px;
    display: inline-block;
    margin-bottom: 10px;
    margin-left: 2px;
}

.captcha-container {
    display: flex;
    align-items: center;
    gap: 5px;
}

.captcha-operator {
    font-size: 18px;
    font-weight: bold;
    color: #333;
}
</style>