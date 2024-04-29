////////////////////////////////////////////////////////////////////////////////////////
//                                                                                    // 
//                             Background Music Player                                //
//                                                                                    //
////////////////////////////////////////////////////////////////////////////////////////

document.addEventListener('DOMContentLoaded', function() {
    var audio = document.getElementById('background_music');
    
    audio.volume = 0.07; // sets the volume
    audio.loop = true; // sets the audio to loop once its finished

    var storedTime = sessionStorage.getItem('audioTime');
    if (storedTime) {
        audio.currentTime = parseFloat(storedTime);
    }

    window.addEventListener('beforeunload', function() {
        sessionStorage.setItem('audioTime', audio.currentTime);
    });
});
