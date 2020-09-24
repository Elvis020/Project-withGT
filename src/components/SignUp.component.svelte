<script>
    let src = '/img/Logo.svg'

</script>

<main>
    <div class="main-container">
    
        <div class="form-container">
            <!-- Image Slide of Black Dispatch -->
            <div class="image-container">
                
            </div>
            <!-- Main Form -->
            <form class="form" action="index.html">
                <img class="logo" {src} alt="Logo">
                <h2 class="sign-up">Sign Up</h2>
                <!-- Name -->
                <div class="input-group">
                    <input type="text" name="name" id="name" autocomplete="off" required>
                    <span></span>
                    <label for="name" class="label-name">
                        Full Name
                    </label>
                </div>

                <!-- Email -->
                <div class="input-group">
                    <input type="text" name="name" id="name" autocomplete="off" required>
                    <span></span>
                    <label for="name" class="label-name">
                        Email
                    </label>
                </div>

                <!-- Password -->
                <div class="input-group">
                     <input type="text" name="name" id="name" autocomplete="off" required>
                     <span></span>
                    <label for="name" class="label-name">
                        Password
                    </label>
                </div>


                <!-- Confirm Password -->
                <div class="input-group">
                    <input type="number" name="name" id="name" autocomplete="off" required>
                    <span></span>
                    <label for="name" class="label-name">
                        Phone Number
                    </label>
                </div>

                <p>By signing up, I accept Black Dispatch's <a href="index.html">Terms of Service</a> and <a href="index.html">Privacy Policy</a></p>

                <button class="submit-button" type="submit">Submit</button>

                <p class="footer">Already have an account? <a href="index.html">SIGN IN</a></p>

            </form>
        </div>
    </div>
</main>


<style>

    /* CSS for main header */
    .logo {
        position: absolute;
        top: 10%;
        left: 50%;
        transform: translate(-50%);
        z-index: 1000;
        width: 50px;
        height: 50px;
    }
    h2{
        margin-bottom: 30px;
    }
    .main-container{
        background: #230de7;
        width: 100%;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .form-container {
        position: relative;
        display: flex;
        background: rgba(191, 194, 47, 0.829);
        border-radius: 10px;
        width: 70%;
        height: 90vh;
        border: none;
        outline: none;
        -webkit-box-shadow: -9px 5px 29px -1px rgba(112,112,112,0.62);
        -moz-box-shadow: -9px 5px 29px -1px rgba(112,112,112,0.62);
        box-shadow: -9px 5px 29px -1px rgba(112,112,112,0.62);

    }

    .form{
        background: #fff;
        position: absolute;
        top: 0;
        right: 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-radius: 0px 10px 10px  0;
        width: 40%;
        height: 100%;
        padding-top: 111px;
    }

    .form .input-group{
        position: relative;

    }
    .form .input-group input {
        width: 250px;
        /* height: 40px; */
        /* padding: 8px 0; */
        font-size: .8em;
        margin-bottom: 25px;
        border: none;
        border-bottom: 1px solid #ccc;
        outline: none;

    }

    .form .input-group label {
        position: absolute;
        color: #333;
        top: 0;
        left: 0;
        /* padding: 7px 0px; */
        font-size: .8em;
        pointer-events: none;
        transition: .3s ease-out
    }

    .input-group span::before {
        content: "";
        position: absolute;
        top: 24.7px;
        left: 0;
        width: 0%;
        height: 2px;
        background: #5fa8d3;
        transition: .3s ease-out
    }

    .input-group input:focus ~ label,
    .input-group input:valid ~ label {
        transform: translateY(-17px);
        font-size: .8rem;
        color: #5fa8d3;
    }
    .input-group input:focus ~ span::before,
    .input-group input:valid ~ span::before{
        width: 100%;
    } 


    .form input:focus +  label::after,
    .form input:valid + label::after{
        transform: translateX(0);
    }




button{
    margin-top: 15px;
    cursor: pointer;
    color: #FFF;
    background: #333;
    border-radius: 15px;
    text-transform: uppercase;
    width: 100px;
    height: 35px;
    -webkit-box-shadow: -1px 9px 42px -12px rgba(0,0,0,0.75);
    -moz-box-shadow: -1px 9px 42px -12px rgba(0,0,0,0.75);
    box-shadow: -1px 9px 42px -12px rgba(0,0,0,0.75);
}

button:focus {
    border: none;
    outline: none;
}

p a{
    color:#39F;
    cursor: pointer;
    text-decoration: none;
}

p{
    font-size: .8rem;
    margin-bottom: 5px;
    text-align: left;
    max-width: 250px;
}

.footer {
    margin-top: 10px;
}


/* CSS of Image Container */

.image-container{
    position: absolute;
    background: green;
    /* z-index: 99; */
    top: 0;
    left: 0;
    border-radius: 10px 0px 0px  10px;
    width: 60%;
    height: 100%;
}

</style>