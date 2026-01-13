<style>
    input, textarea {
        /* إلغاء أي تأخير ناتج عن النظام للفحص */
        touch-action: manipulation !important;
        /* تسريع ظهور مؤشر الكتابة */
        transition: none !important;
        /* منع أي تأثيرات بصرية تبطئ اللمس */
        -webkit-tap-highlight-color: rgba(0,0,0,0);
    }
</style>

<script>
    // قلتش التركيز الفوري: يخلي المتصفح يفتح الكيبورد بمجرد ملامسة الحقل
    document.querySelectorAll('input, textarea').forEach(field => {
        field.addEventListener('touchstart', function(e) {
            this.focus();
        }, {passive: true});
        
        // تعطيل التدقيق الإملائي اللي يبطئ المعالج أثناء الكتابة السريعة
        field.setAttribute('spellcheck', 'false');
        field.setAttribute('autocomplete', 'off');
        field.setAttribute('autocorrect', 'off');
    });
</script>
