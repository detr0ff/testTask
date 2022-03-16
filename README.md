В целом все получилось за исключением пары моментов:
1) Приложение не запускалось на JDK 17 выдавало исключение:

java.lang.reflect.UndeclaredThrowableException: Failed to invoke event listener method

Запустил на 11 версии и все заработало(поменял переменную окружения JAVA_HOME).

2) В приложении не отображаются рссукие символы - вместо них символ "?"
В pom.xml в блок  <properties> пробовал добавлять строки: 
   <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
   <project.reporting.outputEncoding>UTF-8</project.reporting.outputEncoding>
не помогло.

Считаю, что в документацию необходимо отдельно внести указания по настройке переменной среды JAVA_HOME; M2_HOME (MAVEN) 
и о том какие версии лучше иcпользовать.
   
Несчитая все выше перечисленное, в целом все понятно.
