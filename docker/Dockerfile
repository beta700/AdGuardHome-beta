# استخدام الصورة الجاهزة مباشرة بدلاً من محاولة بنائها من الصفر
FROM adguard/adguardhome:latest

# فتح المنافذ الضرورية لـ Render
# المنفذ 853 ضروري جداً ليعمل الـ Private DNS في أندرويد
EXPOSE 53/tcp 53/udp 80/tcp 443/tcp 853/tcp 853/udp 3000/tcp

# تشغيل التطبيق مع ضبط مسارات العمل الافتراضية
ENTRYPOINT ["/opt/adguardhome/AdGuardHome"]
CMD [ \
        "--no-check-update", \
        "-c", "/opt/adguardhome/conf/AdGuardHome.yaml", \
        "-w", "/opt/adguardhome/work", \
        "--host", "0.0.0.0" \
]
