<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>رحلة لمى في القدرات</title>

<style>
* {
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    margin: 0;
    min-height: 100vh;
    background:
        linear-gradient(rgba(15,15,15,.80), rgba(15,15,15,.90)),
        repeating-linear-gradient(
            45deg,
            #263238 0px,
            #263238 20px,
            #303b40 20px,
            #303b40 40px
        );
    color: white;
}

.container {
    width: 92%;
    max-width: 650px;
    margin: auto;
    padding: 25px 0 40px;
}

/* HEADER */

header {
    text-align: center;
    margin-bottom: 25px;
}

.logo {
    font-size: 60px;
    margin-bottom: 5px;
}

h1 {
    margin: 0;
    font-size: 31px;
    color: #7CFC00;
    text-shadow: 3px 3px #111;
}

.subtitle {
    color: #ddd;
    margin-top: 10px;
    line-height: 1.6;
}

/* CARDS */

.card {
    background: rgba(25,25,25,.95);
    border: 3px solid #555;
    border-radius: 12px;
    padding: 20px;
    margin-bottom: 20px;
    box-shadow: 0 7px 0 #111;
}

.card h2 {
    margin-top: 0;
    color: #7CFC00;
}

/* STUDY */

.study-status {
    text-align: center;
}

.check-btn {
    width: 100%;
    border: none;
    border-radius: 8px;
    padding: 18px;
    font-size: 18px;
    font-weight: bold;
    cursor: pointer;
    background: #55a630;
    color: white;
    box-shadow: 0 5px 0 #315c1c;
    transition: .15s;
}

.check-btn:active {
    transform: translateY(4px);
    box-shadow: 0 1px 0 #315c1c;
}

.check-btn.done {
    background: #666;
    box-shadow: 0 5px 0 #444;
    cursor: default;
}

#message {
    display: none;
    margin-top: 20px;
    background: #252525;
    border: 2px dashed #7CFC00;
    padding: 16px;
    border-radius: 8px;
    font-size: 17px;
    line-height: 1.8;
}

/* STREAK */

.streak {
    text-align: center;
    font-size: 26px;
    margin-top: 18px;
}

.streak span {
    color: #ffb703;
    font-weight: bold;
}

/* XP BAR */

.xp-container {
    margin-top: 18px;
    text-align: right;
}

.xp-info {
    display: flex;
    justify-content: space-between;
    margin-bottom: 7px;
    font-size: 14px;
    color: #ccc;
}

.xp-bar {
    width: 100%;
    height: 20px;
    background: #111;
    border: 2px solid #555;
    border-radius: 5px;
    overflow: hidden;
}

.xp-fill {
    height: 100%;
    width: 0%;
    background: #7CFC00;
    transition: width .5s ease;
}

/* LEVEL */

.level {
    text-align: center;
    margin-top: 15px;
    font-size: 18px;
    color: #7CFC00;
}

/* COUNTDOWN */

.countdown {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 8px;
    margin-top: 15px;
}

.time-box {
    background: #151515;
    border: 2px solid #555;
    border-radius: 8px;
    text-align: center;
    padding: 12px 4px;
}

.time-box .number {
    font-size: 24px;
    font-weight: bold;
    color: #7CFC00;
}

.time-box .label {
    font-size: 12px;
    color: #bbb;
    margin-top: 5px;
}

/* TASKS */

.task {
    display: flex;
    align-items: center;
    gap: 10px;
    background: #202020;
    margin: 9px 0;
    padding: 13px;
    border-radius: 8px;
    cursor: pointer;
    transition: .2s;
}

.task:hover {
    background: #2c2c2c;
}

.task input {
    width: 20px;
    height: 20px;
    accent-color: #7CFC00;
}

.task.completed {
    text-decoration: line-through;
    opacity: .55;
}

/* MEMES */

.meme {
    text-align: center;
}

.meme-image {
    width: 100%;
    min-height: 180px;
    border-radius: 10px;
    background:
        linear-gradient(
            135deg,
            #496d2c,
            #27351b
        );
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 75px;
    border: 3px solid #555;
    margin-bottom: 15px;
}

.meme-text {
    font-size: 18px;
    line-height: 1.7;
    white-space: pre-line;
}

.new-meme {
    margin-top: 15px;
    padding: 12px 20px;
    background: #444;
    color: white;
    border: 1px solid #777;
    border-radius: 7px;
    cursor: pointer;
    font-size: 15px;
}

/* FOOTER */

footer {
    text-align: center;
    color: #aaa;
    font-size: 15px;
    margin-top: 30px;
    line-height: 1.8;
}

.footer-love {
    color: #ff9f9f;
    font-size: 17px;
}

footer small {
    color: #777;
}

/* RESET */

.reset {
    text-align: center;
    margin-top: 20px;
}

.reset button {
    background: transparent;
    border: 1px solid #666;
    color: #999;
    padding: 8px 14px;
    border-radius: 6px;
    cursor: pointer;
}

/* MOBILE */

@media (max-width: 450px) {

    h1 {
        font-size: 27px;
    }

    .countdown {
        grid-template-columns: repeat(2, 1fr);
    }

}
</style>
</head>


<body>

<div class="container">

    <!-- HEADER -->

    <header>

        <div class="logo">
            ⛏️
        </div>

        <h1>
            رحلة لمى في القدرات
        </h1>

        <div class="subtitle">
            كل يوم بلوكة جديدة في طريقك للهدف 🧱
            <br>
            لا تستعجلين... أهم شيء تستمرين 💚
        </div>

    </header>


    <!-- STUDY -->

    <div class="card study-status">

        <h2>
            📚 مذاكرة اليوم
        </h2>

        <p id="todayText"></p>

        <button
            id="studyButton"
            class="check-btn"
            onclick="finishStudy()"
        >
            ✅ خلصت مذاكرة اليوم
        </button>


        <div id="message"></div>


        <div class="streak">
            🔥 الستريك:
            <span id="streak">0</span>
            يوم
        </div>


        <!-- XP -->

        <div class="xp-container">

            <div class="xp-info">

                <span id="levelText">
                    المستوى 1
                </span>

                <span id="xpText">
                    0 XP
                </span>

            </div>

            <div class="xp-bar">

                <div
                    id="xpFill"
                    class="xp-fill"
                ></div>

            </div>

        </div>


        <div
            id="levelName"
            class="level"
        >
            🌱 Beginner
        </div>

    </div>



    <!-- COUNTDOWN -->

    <div class="card">

        <h2>
            🎓 العد التنازلي للسنة الدراسية القادمة
        </h2>

        <p>
            باقي على بداية السنة الدراسية:
        </p>

        <div class="countdown">

            <div class="time-box">

                <div
                    class="number"
                    id="days"
                >
                    0
                </div>

                <div class="label">
                    يوم
                </div>

            </div>


            <div class="time-box">

                <div
                    class="number"
                    id="hours"
                >
                    0
                </div>

                <div class="label">
                    ساعة
                </div>

            </div>


            <div class="time-box">

                <div
                    class="number"
                    id="minutes"
                >
                    0
                </div>

                <div class="label">
                    دقيقة
                </div>

            </div>


            <div class="time-box">

                <div
                    class="number"
                    id="seconds"
                >
                    0
                </div>

                <div class="label">
                    ثانية
                </div>

            </div>

        </div>

    </div>



    <!-- TASKS -->

    <div class="card">

        <h2>
            🌱 وش تسوين بعد المذاكرة؟
        </h2>

        <p>
            بعد ما تخلصين قدرات، اختاري الأشياء اللي تبين تسوينها:
        </p>


        <label class="task">

            <input
                type="checkbox"
                onchange="taskDone(this)"
            >

            🚶‍♀️ طلعة أو تمشية بسيطة

        </label>


        <label class="task">

            <input
                type="checkbox"
                onchange="taskDone(this)"
            >

            🎮 لعب ماينكرافت

        </label>


        <label class="task">

            <input
                type="checkbox"
                onchange="taskDone(this)"
            >

            ☕ وقت راحة بدون دراسة

        </label>


        <label class="task">

            <input
                type="checkbox"
                onchange="taskDone(this)"
            >

            🎧 اسمعي أغانيك المفضلة

        </label>


        <label class="task">

            <input
                type="checkbox"
                onchange="taskDone(this)"
            >

            🧹 رتبي غرفتك 10 دقائق

        </label>


        <label class="task">

            <input
                type="checkbox"
                onchange="taskDone(this)"
            >

            📺 شوفي شيء تحبينه

        </label>


        <label class="task">

            <input
                type="checkbox"
                onchange="taskDone(this)"
            >

            💤 نامي بدري وخلي بكرة لبكرة

        </label>

    </div>



    <!-- MINECRAFT MEMES -->

    <div class="card meme">

        <h2>
            ⛏️ Minecraft Meme
        </h2>


        <div
            class="meme-image"
            id="memeEmoji"
        >
            🧱⛏️
        </div>


        <div
            class="meme-text"
            id="memeText"
        >
            لما تقولين بذاكر ساعة...
            وبعد خمس دقايق تعدين كم بلوكة عندك 😂
        </div>


        <button
            class="new-meme"
            onclick="newMeme()"
        >
            😂 ميم ثاني
        </button>

    </div>



    <!-- RESET -->

    <div class="reset">

        <button onclick="resetToday()">
            إعادة ضبط إنجاز اليوم
        </button>

    </div>



    <!-- FOOTER -->

    <footer>

        <div class="footer-love">
            صنع بحب من عبدالله إلى لمى 🍼💚
        </div>

        <small>
            كل يوم بلوكة أقرب لحلمك 🧱⛏️
        </small>

    </footer>

</div>



<script>

/*
==================================================
تاريخ بداية السنة الدراسية القادمة
==================================================

إذا عرفت موعد بداية الجامعة الحقيقي
غيّر التاريخ هنا.

الصيغة:
YYYY-MM-DDTHH:MM:SS

حالياً:
1 سبتمبر 2027 الساعة 8 صباحاً
==================================================
*/

const SCHOOL_START =
    "2027-09-01T08:00:00";



/*
==================================================
رسائل التشجيع
==================================================
*/

const messages = [

    "يا لمى! 🔥 خلصتي مذاكرة اليوم، كفو عليكِ! خطوة صغيرة اليوم = فرق كبير بعدين 💚",

    "تم بناء بلوكة جديدة في طريقك للهدف 🧱⛏️ لا توقفين!",

    "لمى دخلت المود الوحشي اليوم 😎🔥 القدرات ما يدري وش جاه!",

    "كفو! اليوم ما راح يروح بدون إنجاز. فخورة فيكِ 💚",

    "خلصتي؟ أجل اقفلي الكتب وروحي استمتعي شوي 😂 تستاهلين!",

    "كل يوم تذاكرين فيه أنتِ أقرب للدرجة اللي تبينها 🎯",

    "Achievement Unlocked 🏆: مذاكرة اليوم تمت بنجاح!",

    "حتى الـ Creeper ما يقدر يفجر الستريك حقك 💥😂",

    "اليوم مذاكرة، بكرة نتيجة تفرحك بإذن الله 🤍",

    "شغل نظيف يا لمى! ⛏️💚 استمري على نفس الهدوء والاستمرار."

];



/*
==================================================
Minecraft Memes
==================================================
*/

const memes = [

    {
        emoji: "🧟‍♂️⛏️",
        text:
        "لمى: بذاكر قدرات ساعتين.\n\n" +
        "أيضًا لمى بعد 10 دقائق: خلني أحفر شوي 😂"
    },

    {
        emoji: "💎😎",
        text:
        "لما تحلين سؤال صعب من أول محاولة:\n\n" +
        "أنا الآن عندي دايموند 😂💎"
    },

    {
        emoji: "🧱📚",
        text:
        "كل سؤال تحلينه = بلوكة جديدة في بناء مستقبلك 🧱💚"
    },

    {
        emoji: "💥🟩",
        text:
        "السؤال: سهل جدًا.\n\n" +
        "لمى: أكيد فيه Creeper مخبي وراه 😂"
    },

    {
        emoji: "🏠⛏️",
        text:
        "بعد المذاكرة: ألعب شوي.\n\n" +
        "بعد 5 ساعات: بنيت قرية كاملة 😂"
    },

    {
        emoji: "🐷💎",
        text:
        "القدرات: سؤال جديد.\n\n" +
        "لمى: أعطني الـ Diamond Sword 😂"
    },

    {
        emoji: "🧠⛏️",
        text:
        "لما مخك يقول خلاص تعبت...\n\n" +
        "بس باقي سؤال واحد 😭⛏️"
    },

    {
        emoji: "🌳🪓",
        text:
        "دخلت أذاكر قدرات...\n\n" +
        "طلعت أفكر أبني بيت في Minecraft 😂"
    }

];



/*
==================================================
الحصول على تاريخ اليوم
==================================================
*/

function getToday() {

    const now = new Date();

    return now.getFullYear() +
        "-" +
        String(
            now.getMonth() + 1
        ).padStart(2, "0") +
        "-" +
        String(
            now.getDate()
        ).padStart(2, "0");

}



/*
==================================================
عرض تاريخ اليوم
==================================================
*/

function showDate() {

    const date = new Date();

    const options = {

        weekday: "long",

        year: "numeric",

        month: "long",

        day: "numeric"

    };

    document.getElementById(
        "todayText"
    ).textContent =
        date.toLocaleDateString(
            "ar-SA",
            options
        );

}



/*
==================================================
إنهاء مذاكرة اليوم
==================================================
*/

function finishStudy() {

    const today =
        getToday();

    const lastStudy =
        localStorage.getItem(
            "lastStudy"
        );


    /*
    إذا سجلت اليوم بالفعل
    لا نضيف XP مرة ثانية
    */

    if (lastStudy === today) {

        return;

    }


    localStorage.setItem(
        "lastStudy",
        today
    );


    /*
    الستريك
    */

    let streak =
        parseInt(
            localStorage.getItem(
                "streak"
            ) || "0"
        );


    const previousDate =
        localStorage.getItem(
            "previousDate"
        );


    if (previousDate) {

        const yesterday =
            new Date();

        yesterday.setDate(
            yesterday.getDate() - 1
        );


        const yesterdayString =
            yesterday.getFullYear() +
            "-" +
            String(
                yesterday.getMonth() + 1
            ).padStart(2, "0") +
            "-" +
            String(
                yesterday.getDate()
            ).padStart(2, "0");


        if (
            previousDate ===
            yesterdayString
        ) {

            streak++;

        } else {

            streak = 1;

        }

    } else {

        streak = 1;

    }


    localStorage.setItem(
        "streak",
        streak
    );


    localStorage.setItem(
        "previousDate",
        today
    );


    /*
    XP
    */

    let xp =
        parseInt(
            localStorage.getItem(
                "xp"
            ) || "0"
        );


    xp += 100;


    localStorage.setItem(
        "xp",
        xp
    );


    /*
    تحديث الصفحة
    */

    updateProgress();


    /*
    رسالة عشوائية
    */

    const randomMessage =
        messages[
            Math.floor(
                Math.random() *
                messages.length
            )
        ];


    const message =
        document.getElementById(
            "message"
        );


    message.innerHTML =
        "🎉 <strong>تم تسجيل مذاكرة اليوم!</strong>" +
        "<br><br>" +
        randomMessage;


    message.style.display =
        "block";


    /*
    تغيير الزر
    */

    const button =
        document.getElementById(
            "studyButton"
        );


    button.textContent =
        "🎉 تم إنجاز مذاكرة اليوم";


    button.classList.add(
        "done"
    );


    button.disabled = true;

}



/*
==================================================
تحديث XP والمستوى
==================================================
*/

function updateProgress() {

    const xp =
        parseInt(
            localStorage.getItem(
                "xp"
            ) || "0"
        );


    const streak =
        parseInt(
            localStorage.getItem(
                "streak"
            ) || "0"
        );


    /*
    كل 500 XP = مستوى
    */

    const level =
        Math.floor(
            xp / 500
        ) + 1;


    const currentXP =
        xp % 500;


    const percentage =
        (currentXP / 500) * 100;


    document.getElementById(
        "xpText"
    ).textContent =
        currentXP + " / 500 XP";


    document.getElementById(
        "xpFill"
    ).style.width =
        percentage + "%";


    document.getElementById(
        "levelText"
    ).textContent =
        "المستوى " + level;


    document.getElementById(
        "streak"
    ).textContent =
        streak;


    /*
    أسماء المستويات
    */

    let levelName;


    if (level === 1) {

        levelName =
            "🌱 Beginner";

    } else if (level === 2) {

        levelName =
            "⛏️ Miner";

    } else if (level === 3) {

        levelName =
            "🪨 Stone Miner";

    } else if (level === 4) {

        levelName =
            "🔥 Nether Explorer";

    } else if (level === 5) {

        levelName =
            "💎 Diamond Miner";

    } else {

        levelName =
            "👑 Netherite Legend";

    }


    document.getElementById(
        "levelName"
    ).textContent =
        levelName;

}



/*
==================================================
تحميل حالة المذاكرة
==================================================
*/

function loadStudyStatus() {

    const today =
        getToday();


    const lastStudy =
        localStorage.getItem(
            "lastStudy"
        );


    if (
        lastStudy === today
    ) {

        const button =
            document.getElementById(
                "studyButton"
            );


        button.textContent =
            "🎉 تم إنجاز مذاكرة اليوم";


        button.classList.add(
            "done"
        );


        button.disabled = true;


        document.getElementById(
            "message"
        ).innerHTML =
            "💚 كفو يا لمى! أنتِ مخلصة مذاكرة اليوم، الحين وقت الاستراحة والاستمتاع 😎";


        document.getElementById(
            "message"
        ).style.display =
            "block";

    }

}



/*
==================================================
العد التنازلي
==================================================
*/

function updateCountdown() {

    const target =
        new Date(
            SCHOOL_START
        ).getTime();


    const now =
        new Date().getTime();


    const difference =
        target - now;


    if (
        difference <= 0
    ) {

        document.getElementById(
            "days"
        ).textContent = "🎓";


        document.getElementById(
            "hours"
        ).textContent = "بدأت";


        document.getElementById(
            "minutes"
        ).textContent = "🔥";


        document.getElementById(
            "seconds"
        ).textContent = "💚";


        return;

    }


    const days =
        Math.floor(
            difference /
            (1000 * 60 * 60 * 24)
        );


    const hours =
        Math.floor(
            (
                difference /
                (1000 * 60 * 60)
            ) % 24
        );


    const minutes =
        Math.floor(
            (
                difference /
                (1000 * 60)
            ) % 60
        );


    const seconds =
        Math.floor(
            (
                difference /
                1000
            ) % 60
        );


    document.getElementById(
        "days"
    ).textContent =
        days;


    document.getElementById(
        "hours"
    ).textContent =
        hours;


    document.getElementById(
        "minutes"
    ).textContent =
        minutes;


    document.getElementById(
        "seconds"
    ).textContent =
        seconds;

}



/*
==================================================
المهام
==================================================
*/

function taskDone(
    checkbox
) {

    const task =
        checkbox.parentElement;


    if (
        checkbox.checked
    ) {

        task.classList.add(
            "completed"
        );

    } else {

        task.classList.remove(
            "completed"
        );

    }

}



/*
==================================================
تغيير الميم
==================================================
*/

function newMeme() {

    const random =
        memes[
            Math.floor(
                Math.random() *
                memes.length
            )
        ];


    document.getElementById(
        "memeEmoji"
    ).textContent =
        random.emoji;


    document.getElementById(
        "memeText"
    ).textContent =
        random.text;

}



/*
==================================================
إعادة ضبط اليوم
==================================================
*/

function resetToday() {

    const answer =
        confirm(
            "متأكدة تبين تمسحين إنجاز اليوم؟ 😭"
        );


    if (answer) {

        localStorage.removeItem(
            "lastStudy"
        );

        location.reload();

    }

}



/*
==================================================
تشغيل التطبيق
==================================================
*/

showDate();

loadStudyStatus();

updateProgress();

updateCountdown();


/*
العداد يتحدث كل ثانية
*/

setInterval(
    updateCountdown,
    1000
);

</script>

</body>
</html>
