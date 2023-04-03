# How-many-ads-do-we-see-?
Visual analysis of the amount of advertising in the urban environment using computer vision (U-Net + PSP-Net) || Визуальный анализ заполненности городской среды элементами рекламы с помощью компьютерного зрения (U-Net + PSP-Net)

PDF-information with visual materials - https://drive.google.com/file/d/1v0ffq4pYv2SAMInnPkagXIEkRLmf0ife/view?usp=share_link



На основе сегментации изображений проведем анализ количества рекламы в городской среде.Работа включает в себя анализ по следующим пунктам:
- Рекламные экраны,стенды вдоль тротуаров и дорог и т.д.
- Вывески-названия на фасадах зданий.
Из результатов сегментации вычисляется соотношение площади рекламных элементов к площади кадра; Развитие темы взможно в:
- Анализе заполненности элементами рекламы фасадов зданий, являющихся объектом культурного наследия и т.п.(актуально для КГИОП)
- Анализе количества рекламы вдоль дорог - воздействие на фокус внимания водителя.

В Исследовании архитектура нейронной сети основана на комбинации U-Net и PSP-Net, что позволило добиться более четких и явных контуров сегмнентирования.
_______________________________________________________________________________________________________________________________________________________________________

Based on image segmentation, we will analyze the amount of advertising in the urban environment. The work includes an analysis of the following points:
- Advertising screens, stands along sidewalks and roads, etc.
- Signboards-names on the facades of buildings.
From the results of segmentation, the ratio of the area of advertising elements to the area of the frame is calculated; The development of the theme is possible in:
- Analysis of the occupancy of the facades of buildings that are objects of cultural heritage, etc. with advertising elements (relevant for Department of Protection of Cultural and Historical Monuments)
- Analysis of the amount of advertising along the roads - the impact on the focus of the driver's attention.

In the Study, the architecture of the neural network is based on a combination of U-Net and PSP-Net, which made it possible to achieve clearer and more explicit segmentation contours.

_______________________________________________________________________________________________________________________________________________________________________
_______________________________________________________________________________________________________________________________________________________________________

Создана база из 480 фотографий и проведена сегментация изображений:
- Экраны, плакаты, стенды и аналоги сегментированы красным цветом 250,0,0. 
- Текстовые вывески на фасадах сегментированы зеленым цветов 0,250,0.
- Остальная часть фотографии - черным.
Преимущественно угол обзора соответствует 60-80 градусам,при которых человеческое зрение воспринимает символы, также есть расширенный угол, условно соответствующий
углузрения 120 градусов (периферийное зрение),что позволяет провести своего рода анализ того,сколько "лишней" информации мы наблюдаем в городской среде.

Формат изображений PNG, размер 4032х3024.
Проведена аугментация - база расширена до 1.920 кадров. После первого этапа обучения - до 2.400 кадров.
_______________________________________________________________________________________________________________________________________________________________________

A database of 480 photographs was created and image segmentation was carried out:
- Screens, posters, stands and analogues are segmented in red 250.0.0.
- Text signs on the facades are segmented in green 0.250.0.
- The rest of the photo is in black.
Mostly, the viewing angle corresponds to 60-80 degrees, at which human vision perceives symbols, there is also an extended angle, conditionally corresponding to
120 degree vision (peripheral vision), which allows us to conduct a kind of analysis of how much "extra" information we observe in the urban environment.

PNG image format, size 4032x3024
Augmentation was carried out - the base was expanded to 1.920 frames. After the first stage of training - up to 2.400 frames.
