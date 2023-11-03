# HACKATHON_Yandex.Music
### **Цель:** Разработка ML-модели для сопоставления текстов музыкальных произведений и для поиска каверов (вариации обработки оригинала с элементами новой аранжировки) по их текстам

### **Задача**: Разработать ML-продукт, который:

- Находит все кавер-треки и/или исходники к заданному треку в датасете
- Перечисляет все кавер-треки и/или оригиналы к заданному, указывает положение данного трека в цепочке каверов

### **Стек:** *pandas, pyplot, seaborn, sklearn, CatBoost, XGBoost, LightGBM, NLP*

### **Описание данных**

#### Разметка каверов

Файл `covers.json` содержит разметку каверов, сделанную редакторами сервиса:

- `track_id` - уникальный идентификатор трека;
- `track_remake_type` - метка, присвоенная редакторами. Может принимать значения `ORIGINAL` и `COVER`;
- `original_track_id` - уникальный идентификатор исходного трека.

#### Метаинформация

- `track_id` - уникальный идентификатор трека;
- `dttm` - первая дата появления информации о треке;
- `title` - название трека;
- `language` - язык исполнения;
- `isrc` - международный уникальный идентификатор трека;
- `genres` - жанры;
- `duration` - длительность трека;

#### Текст песен

- `track_id` - уникальный идентификатор трека;
- `lyricId` - уникальный идентификатор текста;
- `text` - текст трека.
