# Розділ 7. Побудова моделі даних

Для роботи системи SmartChef визначено наступні основні сутності та атрибути:

1. User (Користувач): id, name, email, password_hash, created_at.
2. Recipe (Рецепт): id, title, description, image_url, instructions, author_id.
3. Favorite (Обране): user_id, recipe_id (зв'язок Many-to-Many).
4. Ingredient (Інгредієнт): id, name, amount, unit, recipe_id.

Зв'язки:
- Один Користувач може мати багато рецептів в "Обраному" (1:N).
- Один Рецепт містить багато інгредієнтів (1:N).
- Рецепти можуть належати конкретним авторам-користувачам.

(ER-діаграма збережена у папці screenshots/er_diagram.jpg)