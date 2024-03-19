# Django Chat Application with Channels and Redis

This Django application provides real-time chat functionality using Django Channels and Redis. It allows users to create chatrooms, send messages, view member counts, send private messages within the chatroom, receive notifications for user join/leave events, and see the list of online members.

## Prerequisites

Before running the application, ensure you have the following installed:

- Python (>=3.6)
- Django (>=3.x)
- Redis (>=5.x)

## Installation

1. Clone this repository to your local machine:

    ```bash
    git clone  https://github.com/talhamsajid/django-chatapp.git
    ```

2. Navigate to the project directory:

    ```bash
    cd django-chat-app
    ```

3. Install Python dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Make migrations and migrate the database:

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

## Configuration

1. Configure Redis:

   - Ensure Redis is running on your system.
   - Update `CHANNEL_LAYERS` settings in `settings.py` to use Redis as the channel layer backend.

2. Configure Django settings:

   - Update `ALLOWED_HOSTS` in `settings.py` with your domain or IP address.
   - Configure any other settings as needed, such as database settings.

## Running the Application

1. Start the Django development server:

    ```bash
    python manage.py runserver
    ```

2. Open your web browser and navigate to `http://localhost:8000` to access the chat application.

## Usage

- **Creating a Chatroom:** Users can create new chatrooms by providing a name and description.
- **Sending Messages:** Users can send messages in the chatroom by typing in the message input field and pressing Enter.
- **Private Messages:** Users can send private messages to other users in the same chatroom by clicking on their username and typing the message in the private message input field.
- **Viewing Member Count:** The application displays the count of members in each chatroom.
- **Notifications:** Users receive notifications when a new user joins or leaves the chatroom.
- **Online Members:** The application always displays a list of online members on the side.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
