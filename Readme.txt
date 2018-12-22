   // Windows Phone must come first because its UA also contains "Android"
    if (/windows phone/i.test(userAgent)) {
        os = "sms:+919171547917?body=" + msg;

    }
    // iOS detection from: http://stackoverflow.com/a/9039885/177710
    if (/iPad|iPhone|iPod/.test(userAgent) && !window.MSStream) {
        os = "sms:+919171547917&body=" + msg;

    }
//Android
    if (/android/i.test(userAgent)) {
        os = "sms:+919171547917?body=" + msg;

    };
