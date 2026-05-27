0. Смонтируйте iso-образ  Matlab914_R2023a_Win64.iso  в виртуальный диск
     На виндовз 8 и ниже для этого может потребоваться программа типа Daemon Tools Lite (или любая подобная)

1. Запустите  setup.exe  на этом виртуальном диске
     Если вы видите запрос логина Mathworks (это происходит когда у установщика есть доступ в интернет)
       то в правом верхнем углу в  "Advanced Options"  выберите режим установки  "I have a File Installation Key"
     Если доступа в интернет установщик не обнаружит, то требуемый режим установки будет выбран автоматом

2. Когда дойдете до  "Enter File Installation Key"  введите  11973-09838-55302-00491-38528-14553-26058-57343-53984-45172-63956-37299
     Если вам нужен  Polyspace          тогда используйте    12149-08760-50815-14586-10614-05215-42250-05782
     Если вам нужен  Polyspace Server   тогда используйте    30971-06149-09640-23099-33091-02284-25342-43212
     Если вам нужен  Parallel Server    тогда используйте    62572-31198-40999-08157-56473-27629-16611-33305-32632-49490-27862-49270
     Если вам нужен  Production Server  тогда используйте    16443-52072-40397-17440-16153
     Если вам нужен  Web App Server     тогда используйте    56905-63171-31644-02067-04593

3. Когда дойдете до  "Select License File"  выберите файл  "license.lic"  из папки с файлом Matlab914_R2023a_Win64.iso

4. Далее выберите и запомните <matlabfolder> - папку куда хотите поставить Матлаб
     По умолчанию это папка  C:\Program Files\Matlab\R2023a

5. Когда дойдете до  "Select products"  поставьте галки на нужных вам компонентах
     Если будет выбрано всё, то Матлаб займет около 25Гигов. Если только  "MATLAB"  то примерно 4Гига
     Поэтому для экономии места и времени запуска отключайте то что вы не знаете или знаете что вам не нужно.
     Матлаб лучше ставить на SSD диск для повышения скорости запуска (а такие диски зачастую "не резиновые"). Так что думайте сами.

6. Когда дойдете до  "Select Options"  выберите галочку  "Add shortcut to desktop"

7. Прогресс установки компонентов может не отображаться корректно (например, всегда показывать 0%) ... просто ждите.
     Если процесс затянулся слишком долго следите растет ли размер папки куда ставите Матлаб
     Если несколько минут размер не растет - перезапустите установку c пункта 1

8. По окончании установки скопируйте файл  "libmwlmgrimpl.dll"  из папки с файлом  Matlab914_R2023a_Win64.iso
     в УЖЕ СУЩЕСТВУЮЩУЮ ПАПКУ  "<matlabfolder>\bin\win64\matlab_startup_plugins\lmgrimpl"
     C ПЕРЕЗАПИСЬЮ УЖЕ СУЩЕСТВУЮЩЕГО ФАЙЛА
     Некоторые ошибаются, выполняя этот пункт невнимательно. Поэтому слова про перезапись написаны большими буквами!!!
     Если при копировании файла вас не спросили про перезапись файла, то вы сделали этот пункт не верно (ну либо Матлаб не установился)!

9. Можно работать :)
     Если установщик не создал ярлык запуска Матлаба на рабочем столе (либо создал неверный ярлык)
     то либо создайте новый ярлык (либо измените неверный) так чтобы ярлык указывал на
     <matlabfolder>\bin\win64\MATLAB.exe


P.S.
Если вам нужна оффлайн (локальная) документация для матлаба то теперь ее надо ставить отдельным действием из  Matlab914Docs
  Пока не поставите локальную документацию любой запрос информации в матлабе будет требовать предоставления ему доступа в интернет

Чтобы дополнить состав компонентов Матлаба надо повторить установку Матлаба выбирая в списке компонентов в установщике только недостающие
  Если вы используете оффлайн документацию то ее установку надо будет тоже повторить

После каждого обновления Матлаба (установки Update'а) пункт 8 надо выполнить повторно!

Если после обновления/дополнения Матлаба начала появляться ошибка при запуске Матлаба то первым делом стоит пробовать повторно выполнить пункт 8




0. Mount iso-file  Matlab914_R2023a_Win64.iso  to virtual disk
     For Windows 8 and lower you probably need soft like Daemon Tools Lite (or similar)

1. Run setup.exe from that virtual disk
     If you see mathworks login/password/signin form (installer has access to internet)
       then in upper right corner in  "Advanced Options"  select setup mode  "I have a File Installation Key"
     If internet access is absent then required setup mode will be auto-selected and you do not need to select it manually

2. When you will be asked to  "Enter File Installation Key"  use  11973-09838-55302-00491-38528-14553-26058-57343-53984-45172-63956-37299
     If you need  Polyspace          then use  12149-08760-50815-14586-10614-05215-42250-05782
     If you need  Polyspace Server   then use  30971-06149-09640-23099-33091-02284-25342-43212
     If you need  Parallel Server    then use  62572-31198-40999-08157-56473-27629-16611-33305-32632-49490-27862-49270
     If you need  Production Server  then use  16443-52072-40397-17440-16153
     If you need  Web App Server     then use  56905-63171-31644-02067-04593

3. When you will be asked to  "Select License File"  select file  "license.lic"  from folder with  Matlab914_R2023a_Win64.iso  file

4. Then select and remember <matlabfolder> - folder where you want Matlab to be installed
     Default is  "C:\Program Files\MATLAB\R2023a"

5. When you will be asked to  "Select products"  select components you need
     If you all components are selected Matlab will need about 25Gb of disk space and somewhat longer startup time
     If you select only  "MATLAB"  then Matlab will need about  4Gb of disk space
     You better install Matlab on SSD disk for better startup time, so most likely you do not want to waste SSD-disk space for nothing

6. Then in  "Select Options"  select  "Add shortcut to desktop"

7. Components setup progress may be shown incorrectly (for example always show 0%) ... just wait
     Or if installation process takes too long start to monitor size of <matlabfolder> folder
     If the size is not growing after several minutes then restart setup from step 1

8. After installation is done copy file  "libmwlmgrimpl.dll"  from folder with  Matlab914_R2023a_Win64.iso  file
     to ALREADY EXISTING FOLDER  "<matlabfolder>\bin\win64\matlab_startup_plugins\lmgrimpl"
     WITH OVERWRITING OF EXISTING FILE
     If you was NOT asked about overwriting then you are doing something wrong (or Matlab was not installed successfully)!!!

9. Work with Matlab :)
     If desktop shortcut was not created (or was created bad shortcut)
     then create new shortcut (or change existing one) so that it run the
     "<matlabfolder>\bin\win64\MATLAB.exe"


P.S.
If you need offline (local) documentation for matlab then you need to install it separately from  Matlab914Docs
  Until you install offline documentation any information request inside matlab will require internat access

To extend set of installed Matlab components you need to repeat Matlab installation selecting in installer only currently absent components
  If you use offline documentation then you need to repeat its installation too

After every update of Matlab you need to reexecute step 8

If after update/change of Matlab you get error during startup of Matlab then first try to redo the step 5
