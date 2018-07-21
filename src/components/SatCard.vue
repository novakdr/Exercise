<template>
    <div class='sat-card'>
        <div class='info'>
            <h2 class='name'>Sat</h2>
            <h4 class='location'>on-campus</h4>
            <h4 class='type'>Practice Exam</h4>
            <h4 class='time'>05.12.2018</h4>
            <button>learn More</button>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['result']
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sat-card {
    background: salmon;
    color: white;
    padding: 30px 20px;
    padding-bottom: 20px;
    margin: 10px;
    display: flex;
    flex-grow: 1;
}

.info {
    max-width: 250px;
}

h2 {
    margin: 0;
    padding: 0;
    line-height: 1;
}

h4 {
    margin: 0;
    padding: 0;
    line-height: 1;
}

.name {
    font-size: 3rem;
    font-weight: 800;
    text-transform: uppercase;
}

.location {
    text-transform: uppercase;
    font-weight: 200;
    font-size: 2rem;
    line-height: .8;
}

.type {
    font-size: 2rem;
    text-transform: uppercase;
    font-weight: 800;
}

.time {
    font-size: 2rem;
    text-transform: uppercase;
    font-weight: 800;
}

button {
    background: white;
    color: salmon;
    border: none;
    padding: .5rem 1.2rem;
    text-transform: uppercase;
    font-weight: 800;
    font-size: .8rem;
    margin-top: 10px;
}

button:hover {
    cursor: pointer;
}

/* 576 or Smaller Media Query */
@media (max-width: 575px) {
    .sat-card {
        padding: 20px 10px;
        padding-bottom: 10px;
        margin: 5px;
    }

    .name {
        font-size: 2.3rem;
        font-weight: 800;
        text-transform: uppercase;
    }

    .location {
        font-size: 1.3rem;
    }

    .type {
        font-size: 1.3rem;
    }

    .time {
        font-size: 1.3rem;
    }

    button {
        font-size: .4rem;
    }
}

/* 576 Media Query */
@media (min-width: 576px) {
    .sat-card {
        padding: 20px 10px;
        padding-bottom: 10px;
        margin: 5px;
    }

    .name {
        font-size: 2.7rem;
        font-weight: 800;
        text-transform: uppercase;
    }

    .location {
        font-size: 1.7rem;
    }

    .type {
        font-size: 1.7rem;
    }

    .time {
        font-size: 1.7rem;
    }

    button {
        font-size: .4rem;
    }
}

/* 768 Media Query */
@media (min-width: 768px) {
    .sat-card {
        padding: 20px 10px;
        padding-bottom: 10px;
        margin: 5px;
    }

    .name {
        font-size: 2.3rem;
        font-weight: 800;
        text-transform: uppercase;
    }

    .location {
        font-size: 1.3rem;
    }

    .type {
        font-size: 1.3rem;
    }

    .time {
        font-size: 1.3rem;
    }

    button {
        font-size: .4rem;
    }
}

/* 992 Media Query */
@media (min-width: 992px) {
    .name {
        font-size: 2.7rem;
        font-weight: 800;
        text-transform: uppercase;
    }

    .location {
        font-size: 1.7rem;
    }

    .type {
        font-size: 1.7rem;
    }

    .time {
        font-size: 1.7rem;
    }

    button {
        font-size: .7rem;
    }
}

/* 1200 Media Query */
@media (min-width: 1200px) {
    .name {
        font-size: 3rem;
        font-weight: 800;
        text-transform: uppercase;
    }

    .location {
        font-size: 2rem;
    }

    .type {
        font-size: 2rem;
    }

    .time {
        font-size: 2rem;
    }

    button {
        font-size: .8rem;
    }
}
</style>
