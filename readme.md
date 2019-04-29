Рассматриваемые деревья:
* Spruce/Fir (елово-пихтовые)
* Lodgepole Pine (сосна скрученная)
* Ponderosa Pine (сосна жёлтая)
* Cottonwood/Willow (ива)
* Aspen (осина)
* Douglas-fir (псевдотсуга Мензиса)
* Krummholz (криволесье) <br>

В  ходе анализа было замечено в данных:
* различное распределение параметра elevation
* различные пропорции каждого из типов деревьев в исследуемых регионах
* различные пропорции каждого из типов деревьев для каждого из видов почв <br>
[Вдохновение №1](https://www.fs.fed.us/psw/publications/north/psw_2016_north005.pdf) <br>
[Вдохновение №2](https://www.photopills.com/articles/understanding-azimuth-and-elevation) <br>
Варианты использования признаков:
* точно не использовать: Wilderness Area, Horizontal Distance To Roadways, Horizontal Distance To Fire Points исходя из данной статьи
* вертикальное и горизонтальное расстояния объеденить в новый признак - евклидово расстояние до воды
* группировка типа почв: dry, wet, stony or rock
* исходя из [данной статьи](http://desktop.arcgis.com/ru/arcmap/10.3/tools/spatial-analyst-toolbox/how-hillshade-works.htm) существует связь между slope, aspect & hillshade. 
* логично, что параметры hillshade 9am, noon, 3pm также влияют на целевой класс в совокупности (в зависимости от типа кроны дерева эти параметры могут отличаться) => стоит ввести ещё один признак hillshade_avg
