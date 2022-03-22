/*OpenSea*/

.wave-btn{
    width: 280px;
    height: 60px;
    display: flex;
    border-radius: 0 0 10px 10px;
    justify-content: center;
    align-items: center;
    transition: all 0.8s ease 0s;
    text-decoration: none;
    position: relative;
    margin-left: 50em;
    overflow: hidden;
}


.wave-btn:hover .wave-btn_waves{
    top: -50px;
}

.wave-btn_text{
    color: #fff;
    
    letter-spacing: 8px;
    position: relative;
    z-index: 1;
}

.wave-btn:hover{
    border-radius: 10px;
    transition: all 0.8s ease 0.2s;

    box-shadow: inset 0 0 40px rgba(255, 99, 71, 0.6);
}

.wave-btn_waves{
    position: absolute;
    width: 280px;
    height: 280px;
    background: url("../images/intro.jpg") center no-repeat;
    -webkit-background-size: cover;
    background-size: cover;
    top: 0;
    box-shadow: inset 0 0 50px rgba(0, 0, 0, 0.5);
    transition: all 0.8s ease 0s;
}

.wave-btn_waves:after,
.wave-btn_waves:before{
    content: '';
    position: absolute;
    top: 0;
    left: 50%;
    width: 250%;
    height: 250%;
    transform: translate3d(-50%,-96%,0) rotate(0deg) scale(1);
}

.wave-btn_waves:before{
    background-color: rgba(255, 99, 71);
    border-radius: 48%;

    animation: waves 8s infinite linear;
}

.wave-btn_waves:after{
    background: rgba(255, 99, 71, 0.5);
    border-radius: 44%;

    animation: waves 10s infinite linear;
}

@keyframes waves{
    0%{
        transform: translate3d(-50%,-96%,0) rotate(0deg) scale(1);
    }
    100%{
        transform: translate3d(-50%,-96%,0) rotate(360deg) scale(1);
    }
}


            <a href="http://test1.ru/PacificBirds/discord.html" target="_blank" class="wave-btn">
              <span class="wave-btn_text">Buy on OpenSea</span>
              <span class="wave-btn_waves"></span>
            </a>
