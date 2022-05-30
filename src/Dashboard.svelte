<div class="dashboard">
    <header class="waterConsumption">
        <h1>WATER CONSUMPTION</h1>
        <div>
            <p>Last 6 Mounths</p>
            <img src="/images/icons/dashboard/arrowDown.svg" alt="Arrow" />
        </div>
    </header>
    <div class="waterChart">
        <img src="/images/icons/dashboard/waterChart.svg" alt="Water" />
        <div class="waterChartCategories">
            <p>Consumed</p>
            <p>Collected from rain</p>
        </div>
    </div>
    <header class="energyConsumption">
        <h1>ENERGY CONSUMPTION</h1>
        <div>
            <p>Last 6 Mounths</p>
            <img src="/images/icons/dashboard/arrowDown.svg" alt="Arrow" />
        </div>
    </header>
    <div class="energyChart">
        <img src="/images/icons/dashboard/energyChart.svg" alt="Energy" />
        <div class="energyChartCategories">
            <p>Regular Energy</p>
            <p>Generated Solar Power</p>
        </div>
    </div>
</div>

<style>
    .dashboard {
        grid-area: main;
        padding: 34px 40px;
    }
    .dashboard .waterConsumption,
    .dashboard .energyConsumption {
        display: flex;
        flex-direction: column;
    }
    .dashboard .waterConsumption h1,
    .dashboard .energyConsumption h1 {
        margin-bottom: 20px;
    }
    .dashboard .waterConsumption div,
    .dashboard .energyConsumption div {
        display: flex;
        padding: 15px;
        border: 2px solid black;
        cursor: pointer;
        width: 100%;
        justify-content: space-between;
        margin-bottom: 30px;
    }
    .dashboard .waterConsumption div p,
    .dashboard .energyConsumption div p {
        margin-right: 14.5px;
    }
    .waterChart,
    .energyChart {
        margin-bottom: 66px;
    }
    .waterChart img,
    .energyChart img {
        width: 100%;
        margin-bottom: 29px;
    }
    .waterChartCategories,
    .energyChartCategories {
        display: flex;
        align-items: center;
        margin-left: 35px;
    }
    .waterChartCategories p:first-child,
    .waterChartCategories p:last-child {
        display: flex;
        align-items: center;
    }
    .waterChartCategories p:first-child {
        margin-right: 26px;
    }
    .waterChartCategories p:first-child::before,
    .waterChartCategories p:last-child::before {
        content: "";
        display: inline-block;
        align-items: center;
        width: 20px;
        height: 20px;
        border-radius: 50%;
        margin-right: 5px;
    }
    .waterChartCategories p:first-child::before {
        border: 1px solid black;
        background-color: transparent;
    }
    .waterChartCategories p:last-child::before {
        border: 1px solid #ffc4c4;
        background-color: transparent;
    }
    .energyChartCategories p:first-child,
    .energyChartCategories p:last-child {
        display: flex;
        align-items: center;
    }
    .energyChartCategories p:first-child {
        margin-right: 26px;
    }
    .energyChartCategories p:first-child::before,
    .energyChartCategories p:last-child::before {
        content: "";
        display: inline-block;
        align-items: center;
        width: 20px;
        height: 20px;
        border-radius: 50%;
        margin-right: 5px;
    }
    .energyChartCategories p:first-child::before {
        background-color: black;
    }
    .energyChartCategories p:last-child::before {
        background-color: #ffc4c4;
    }
    @media (min-width: 660px) {
        .dashboard .waterConsumption,
        .dashboard .energyConsumption {
            flex-direction: row;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 36px;
        }
        .dashboard .waterConsumption h1,
        .dashboard .energyConsumption h1 {
            margin-bottom: 0;
        }
        .dashboard .waterConsumption div,
        .dashboard .energyConsumption div {
            width: auto;
        }
    }
</style>
