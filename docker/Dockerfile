
FROM adguard/adguardhome:latest

# فتح المنفذ 10000 الذي تستخدمه Render مجاناً
EXPOSE 10000

# تشغيل AdGuard وإجباره على استخدام المنفذ 10000 بدلاً من 80 المعطل
CMD ["/opt/adguardhome/AdGuardHome", "--web-addr", "0.0.0.0:10000", "--no-check-update"]
