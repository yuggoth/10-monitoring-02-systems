# 10.02. Системы мониторинга

## 1 задание
	
Т.к. push использует UDP, то плюс в том, что он работает быстрее. Есть и минусы: возможны потери данных и их подлинность под сомнением, потому что данные может прислать кто угодно.
Pull более надежен и безопасен, т.к. система сама обходит агентов и собирает логи, которые они накопили, но накладные расходы на установление сессий делают этот способ более медленным чем push.

## 2 задание

Prometheus - pull. Можно переделать в push с помощью сервиса pushgateway;

TICK - push;

Zabbix - гибридный. Из коробки работает как push, но может работать и как pull;

VictoriaMetrics - гибридный;

Nagios - pull.
