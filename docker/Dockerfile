FROM adguard/adguardhome:latest

# إجبار واجهة التحكم والويب على المنفذ 3000 المتوافق مع Render
EXPOSE 3000

# تشغيل التطبيق مع تحديد المنفذ 3000 مباشرة في الأمر
CMD ["/opt/adguardhome/AdGuardHome", "--web-addr", "0.0.0.0:3000", "--no-check-update"]
