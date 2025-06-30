Для тренировки весов нужно скачать датасеты по ссылке: https://pjreddie.com/projects/mnist-in-csv/ и закинуть в эту папку.

и https://github.com/phoebetronic/mnist?tab=readme-ov-file

Traceback (most recent call last):
  File "C:\python\digits-recognizer\Neuron_training.py", line 51, in <module>
    inputs_list=(np.asfarray(line[1:])/255*0.99)+0.01
  File "C:\python\digits-recognizer\venv\lib\site-packages\numpy\__init__.py", line 427, in __getattr__
    raise AttributeError(
AttributeError: `np.asfarray` was removed in the NumPy 2.0 release. Use `np.asarray` with a proper dtype instead.