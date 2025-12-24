# استخدام الصورة الجاهزة مباشرة لتجنب أخطاء بناء كود Go
FROM adguard/adguardhome:latest

# فتح المنافذ المطلوبة
EXPOSE 3000 80 443 853 53/udp 53/tcp

# تشغيل البرنامج
ENTRYPOINT ["/opt/adguardhome/AdGuardHome"]
CMD ["--web-addr", "0.0.0.0:3000", "--no-check-update"]
