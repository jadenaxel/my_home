<div class="profile">
    <div class="profile-header">
        <img src="/images/icons/profile/notification.svg" alt="Notify" />
        <div class="profile-header-profile">
            <p class="profile-header-profile-title">Alicia</p>
            <img src="/images/icons/profile/Avatar.svg" alt="Avatar" />
        </div>
    </div>
    <div class="profile-search-task">
        <img src="/images/icons/profile/Search.svg" alt="Search" />
        <input type="text" placeholder="Search tasks to do or help" />
    </div>
    <div class="profile-weather">
        <div class="profile-weather-temperature">
            <img src="/images/icons/profile/arranged.svg" alt="Temperature" />
            <p class="profile-weather-temperature-title">Temperature</p>
            <p class="profile-weather-temperature-text">25°</p>
        </div>
        <div class="profile-weather-humidity">
            <img src="/images/icons/profile/water.svg" alt="Humidity" />
            <p class="profile-weather-humidity-title">Humidity</p>
            <p class="profile-weather-humidity-text">20%</p>
        </div>
    </div>
    <div class="profile-quick">
        <p class="profile-quick-title">QUICK ACCESS</p>
        <div class="profile-quick-access">
            <div class="profile-quick-access-security">
                <div class="profile-quick-access-security-imageContainer">
                    <img src="/images/icons/profile/lock.svg" alt="Lock" />
                </div>
            </div>
            <div class="profile-quick-access-security-data">
                <p class="profile-quick-access-security-data--title">
                    SECURITY
                </p>
                <div class="profile-quick-access-security-data--description">
                    Partial Lock
                </div>
            </div>
        </div>
        <div class="profile-quick-bulb">
            <div class="profile-quick-bulb-light">
                <img src="/images/icons/profile/bulb.svg" alt="Bulb" />
            </div>
            <div class="profile-quick-bulb-data">
                <p class="profile-quick-bulb-data--title">Lights</p>
                <div class="profile-quick-buld-data-state">
                    <div class="profile-quick-buld-data-state-1">
                        <div class="profile-quick-buld-data-state-1--number">
                            <p>3</p>
                            <div />
                        </div>
                        <p>ON</p>
                    </div>
                    <div class="profile-quick-buld-data-state-2">
                        <div class="profile-quick-buld-data-state-2--number">
                            <p>8</p>
                            <div />
                        </div>
                        <p>OFF</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="profile-quick-wifi">
            <div class="profile-quick-wifi-bubble">
                <img src="/images/icons/profile/wifi.svg" alt="Wifi" />
            </div>
            <div class="profile-quick-wifi-data">
                <p class="profile-quick-wifi-data--title">Wifi</p>
                <p class="profile-quick-wifi-device-quantity">4</p>
                <p class="profile-quick-wifi-device-title">Devices</p>
            </div>
        </div>
        <div class="profile-quick-add">
            <div class="profile-quick-add-imageContainer">
                <img src="/images/icons/profile/add.svg" alt="Add" />
            </div>
            <p class="profile-quick-add-title">Add</p>
        </div>
    </div>
</div>

<style>
    .profile {
        grid-area: profile;
        background-color: #fff2f2;
        padding: 44px 36px;
        overflow-y: auto;
        min-height: 100vh;
        display: none;
    }
    .profile::-webkit-scrollbar {
        width: 10px;
    }
    .profile::-webkit-scrollbar-track {
        background: black;
    }
    .profile::-webkit-scrollbar-thumb {
        background-color: #fff2f2;
        border-radius: 20px;
        border: 3px solid black;
    }
    .profile-header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin-bottom: 17px;
    }
    .profile-header > img {
        cursor: pointer;
    }
    .profile-header-profile {
        display: flex;
        align-items: center;
    }
    .profile-header-profile-title {
        font-size: 21px;
    }
    .profile-header-profile img {
        cursor: pointer;
        margin-left: 21px;
    }
    .profile-search-task {
        border: 2px solid black;
        padding: 13px 26px;
        display: flex;
        align-items: center;
        margin-bottom: 39px;
    }
    .profile-search-task img {
        margin-right: 10px;
    }
    .profile-search-task input {
        border: none;
        background-color: transparent;
        font-size: 15px;
    }
    .profile-search-task input:focus {
        outline: none;
    }
    .profile-weather {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
        align-items: center;
        margin-bottom: 67px;
    }
    .profile-weather-temperature-title,
    .profile-weather-humidity-title {
        font-size: 11px;
        font-weight: bold;
    }
    .profile-weather-temperature-text,
    .profile-weather-humidity-text {
        font-weight: bold;
        font-size: 40px;
    }
    .profile-quick-title {
        font-size: 29px;
        margin-bottom: 35px;
    }
    .profile-quick-access,
    .profile-quick-bulb,
    .profile-quick-wifi {
        display: flex;
        align-items: center;
        border-bottom: 1px solid black;
        padding-bottom: 20px;
        margin-bottom: 14px;
    }
    .profile-quick-access-security-imageContainer,
    .profile-quick-bulb-light,
    .profile-quick-wifi-bubble,
    .profile-quick-add-imageContainer {
        width: 70px;
        height: 70px;
        background-color: black;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-right: 34px;
    }
    .profile-quick-access-security-data--title,
    .profile-quick-bulb-data--title,
    .profile-quick-wifi-data--title {
        font-size: 15px;
        font-weight: bold;
        margin-bottom: 6px;
    }
    .profile-quick-bulb {
        display: flex;
        align-items: center;
    }
    .profile-quick-bulb-data {
        display: flex;
        flex-direction: column;
    }
    .profile-quick-buld-data-state {
        display: flex;
    }
    .profile-quick-buld-data-state-1--number,
    .profile-quick-buld-data-state-2--number {
        display: flex;
    }
    .profile-quick-buld-data-state-1--number,
    .profile-quick-buld-data-state-2--number {
        display: flex;
        align-items: center;
    }
    .profile-quick-buld-data-state-1--number {
        margin-right: 18px;
    }
    .profile-quick-buld-data-state-1--number p,
    .profile-quick-buld-data-state-2--number p {
        font-size: 40px;
        font-weight: bold;
        margin-right: 7px;
    }
    .profile-quick-buld-data-state-1--number div,
    .profile-quick-buld-data-state-2--number div {
        width: 12px;
        height: 12px;
        border-radius: 50%;
        border: 2px solid black;
    }
    .profile-quick-buld-data-state-1--number div {
        background-color: #ffc4c4;
    }
    .profile-quick-buld-data-state-2--number div {
        background-color: #ebecf0;
    }
    .profile-quick-wifi-device-quantity {
        font-size: 40px;
        font-weight: bold;
    }
    .profile-quick-wifi-device-title,
    .profile-quick-add-title {
        font-size: 15px;
        font-weight: bold;
    }
    .profile-quick-add {
        display: flex;
        align-items: center;
    }
    @media (min-width: 1120px) {
        .profile {
            display: block;
        }
    }
</style>
