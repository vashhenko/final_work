<style>
    :root {
    --primary-color: rgb(155, 213, 252);
    --secodary-color: rgb(103, 170, 247);
}

* {
    box-sizing:  border-box;
}

main {
    display: flex;
    flex-wrap: wrap;
}











.movie {
    width: 300px;
    margin: 10px;
    background-color: var(--secodary-color);
    box-shadow: 0 4px 5px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}



.movie-info {
    color: black;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px 30px 30px;
    letter-spacing: 0.5px;
}

.movie-info h3{
    margin-top: 0;
}

.movie-info span{
    background-color: var(--primary-color);
    padding: 25px 5px;
    border-radius: 3px;
    font-weight: bold;
}

.movie-info span.green{
    color: lightgreen;
}

.overview {
    background-color: white;
    padding: 20px;
    position: absolute;
    left: 0;
    bottom: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(101%);
    transition: transform 0.3s ease-in;
}

.movie:hover .overview{
    transform: translateY(0)
}
</style>

<main id="main">
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Крепкий Орешек</h3>
            <span class="green">9.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
        </div>
    </div>

    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Не Крепкий Орешек</h3>
            <span class="green">8.0</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
        </div>
    </div>

    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Мега не Крепкий Орешек</h3>
            <span class="green">8.7</span>
        </div>
        <div class="overview">
            <h3 id="Description">Описание фильма</h3>
        </div>
    </div>
</main>