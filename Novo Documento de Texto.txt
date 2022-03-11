const BASE_URL = 'https://thatcopy.pw/catapi/rest/'

function recuperarGatos() {
    fetch(BASE_URL)
        .then(callback)
        .catch(tratarError)
}

function callback(gatos) {
    console.log(gatos)
}

function tratarError(error) {
    console.log(error)
}

recuperarGatos()
