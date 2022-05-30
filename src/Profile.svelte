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
</div>

<style>
    .profile {
        background-color: #fff2f2;
        padding: 44px 36px;
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
</style>
