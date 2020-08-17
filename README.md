# AC-VO-PPR-Hackathon
took part in russian hachathon which was arrenged by AC-VO (Акселиратор Возможностей) and PPR (Програмный Продукт))


Name of our team: 
Dream Team


Participants: 
https://github.com/andrei-iliukhin;
https://github.com/BormS;
https://github.com/Dmitry9889.



Кейс: 
Анализ Поведения Пользоватей в Сети


Цель: 
Реализовать модуль анализа трафика, позволяющий выявлять вредоносные соединения на базе анализа логов.


Задачи: 
1.Обнаружить атаки в тестовой выборке и классифицировать их
2.Построить статистику по выявленным атакам, процентные соотношения между атаками
3.Продемонстрировать работу разработанного модуля на реальных данных


Входные Данные: 
1 Наборы данных;
2. Типы тренировочных атак;
3. Схема данных набора данных в машино-читаемой форме;
4. Полный набор данных для обучения;
5. Набор данных для тестирования.


Описание Ситуация

Программное обеспечение для обнаружения сетевых вторжений защищает компьютерную сеть от неавторизованных пользователей.
Задача обучения детектора вторжений состоит в том, чтобы построить прогностическую модель (классификатор), способную различать «плохие» соединения, называемые атаками и «хорошие» нормальные соединения.
Атаки делятся на четыре основные категории:
1. DOS (denial-of-service,): отказ в обслужи-вании;
2. R2L: несанкционированный доступ с удален-ного компьютера, например, угадывание пароля;
3. U2R: несанкционированный доступ к локаль-ным правам суперпользователя (root), например, различные «переполнения буфера»;
4. Зондирование: мониторинг, напри-мер, ска-нирование портов.

Данные теста не имеют того же распределения вероятностей, что и данные обучения, и включают конкретные типы атак, которых нет в данных обучения.
Наборы данных содержат в общей сложности 24 типа тренировочных атак, и дополнительно 14 типов только в тестовых данных.
Некоторые пробные атаки сканируют хосты (или порты) с использованием гораздо большего интервала времени, чем две секунды, например, один раз в минуту. Поэтому записи о соединениях также сортировались по хосту назначения, а функции создавались с использованием окна из 100 соединений с одним хостом вместо временного окна. Это дает набор так называемых функций трафика на основе хоста. В отличие от большинства DOS и зондирующих атак, в записях атак R2L и U2R отсутствуют последовательные шаблоны.       Это связано с тем, что атаки DOS и зондирование вовлекают множество соединений с некоторыми хостами за очень короткий период времени. Атаки R2L и U2R встроены в части данных пакетов и обычно включают только одно соединение.



Case: 
Analysis of User Behavior on the Web


Objective: 
Implement a traffic analysis module that allows detecting malicious connections based on log analysis.


Tasks: 
1. To detect attacks in the test sample and classify them
2. Build statistics on detected attacks, percentages between attacks
3. Demonstrate the work of the developed module on real data
  
  
Input Data: 
1. Data Sets;
2. Types of training attacks;
3. Data schema of the dataset in machine-readable form;
4. Complete set of data for training;
5. Data set for testing.


Description of Situation

Network intrusion detection software protects network from unauthorized users.

The task of training an intrusion detector is to build a predictive model (classifier) that can distinguish between “bad” connections, called attacks, and “good” normal connections.

Attacks fall into four main categories:
1. DOS (denial-of-service,): denial of service;
2. R2L: unauthorized access from a remote computer, for example, guessing a password;
3. U2R: unauthorized access to local superuser (root) rights, for example, various "buffer overflows";
4. Probing: monitoring, for example, port scanning.


The test data does not have the same probability distribution as the training data and includes specific types of attacks that are not in the training data.
The datasets contain a total of 24 types of training attacks, with an additional 14 types in test data only.
Some probe attacks scan hosts (or ports) using a much longer time interval than two seconds, such as once a minute. Therefore, connection records were also sorted by destination host, and functions were created using a window of 100 single host connections instead of a time window. This provides a set of so-called host-based traffic functions. Unlike most DOS and probe attacks, there are no sequential patterns in the R2L and U2R attack records. This is because DOS attacks and probing involve many connections to some hosts in a very short period of time. R2L and U2R attacks are embedded in data portions of packets and usually involve only one connection.
            
            
            
