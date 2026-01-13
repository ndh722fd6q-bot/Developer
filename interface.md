<style>
    .glitch-container {
        text-align: center;
        padding: 20px;
        font-family: sans-serif;
    }
    .glitch-image {
        max-width: 100%;
        height: auto;
        border-radius: 15px;
        box-shadow: 0 4px 15px rgba(0,0,0,0.3);
        margin-bottom: 20px;
        /* منع التأخير عند لمس الصورة */
        touch-action: manipulation;
    }
    .description {
        color: #fff;
        background: #222;
        padding: 10px;
        border-radius: 8px;
        display: inline-block;
    }
</style>

<div class="glitch-container">
    <h2 style="color: #f00;">🚀 شرح قلتش التخفي (The Alias Glitch)</h2>
    
    <img src="رابط_الصورة_الأولى_هنا" alt="شرح القلتش" class="glitch-image">
    
    <div class="description">
        <p>تغيير اسم الملف إلى UnityFramework يخدع الـ Anti-Cheat</p>
    </div>

    <hr style="border: 0.5px solid #444; margin: 30px 0;">

    <img src="رابط_الصورة_الثانية_هنا" alt="تطبيق القلتش" class="glitch-image">
</div>

<script>
    // قلتش السرعة اللي اتفقنا عليه
    document.querySelectorAll('img').forEach(img => {
        img.addEventListener('touchstart', function() {
            console.log('Image touched instantly!');
        }, {passive: true});
    });
</script>
