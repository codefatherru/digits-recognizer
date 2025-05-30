# DigitRecognizer

### Полносвязная нейронная сеть, распознающая числа от 0 до 9

## Скрипты

`Neuron_training.py`- скрипт, в котором происходит обучение сети. Обученные веса csv формата хранятся в папке "weights".

>(Постскриптум, веса уже готовы, ничего обучать не надо. Но если хочется, то нужно скачать MNIST датасет по ссылке: "https://pjreddie.com/projects/mnist-in-csv/"
>, закинуть в папку "dataset", запустить `Neuron_training.py` и подождать некоторое время)

`main.py` - обученная сеть с интерфейсом, которая берет готовые веса и распознаёт числа. 

Сеть обучена на 97 процентов согласно тестовым данным.

## Зависимости
* numpy   v2.0.2
* Pillow  v8.0.1
* tkinter
* pyinstaller

> pip install requirements.txt -r

Так как это полносвязная нейросеть, то она чувствительна к расположению объекта, его размеру и углу наклона. То есть правильно распознавать изображения она будет лишь в том случае, если вышеуказанные параметры будут совпадать с параметрами в датасете.

## Сборка в EXE 

>  pyinstaller   --onefile --name arabian --noconsole .\main.py  

файл arabian.exe будет создан в папке ./dist

для работы нужно скопировать папку ./weights  в ./dist

@todo надо научиться копировать папку weights в дистирбутив. --add-data  ?

для отладки нужно оставить окно консоли:

>  pyinstaller   --onefile --name arabian --add-data  .\main.py  

## YouTube:
[![YouTube](http://img.youtube.com/vi/qnwWK3zlI8Q/0.jpg)](http://www.youtube.com/watch?v=qnwWK3zlI8Q)
