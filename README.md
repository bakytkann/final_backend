# SmartBlog

SmartBlog is an intelligent Flask-based blog that allows users to publish posts with images, automatically generates tags, and analyzes the emotional tone of text using AI models.

---

## Features

**🧠 AI Features**
- Automatic tag generation using KeyBERT
- Analysis of top-3 emotions in text (GoEmotions model)

**📝 Posts**
- Creation, viewing, and deletion of posts
- Image uploads
- Convenient display of tags and emotions in UI

**🔒 Authentication**
- User registration and login

**🎨 UI**
- Modern design for tags and emotions
- Responsive Bootstrap interface

---

## Technologies

- **Backend**: Flask, SQLAlchemy, Flask-WTF
- **AI/NLP**: KeyBERT, SentenceTransformers, GoEmotions (transformers)
- **Frontend**: Jinja2 + Bootstrap
- **Additional Libraries**: WTForms, python-dotenv

---

## Project Structure

```
/blog-project
│
├── app.py                
├── config.py            
├── models.py           
├── forms.py              
├── ai_utils.py         
├── utils.py  
├── extensions.py   
│
├── /instance
│   ├── site.db
│
├── /templates            
│   ├── base.html
│   ├── dashboard.html
│   ├── view_post.html
│   ├── edit_prodile.html
│   ├── login.html
│   ├── register.html
│   ├── profile.html
│   └── create_post.html
│
├── /routes
│   ├── __init__.py
│   ├── auth.py
│   └── posts.py
│
├── /static/uploads       
└── requirements.txt      
```

---

## Installation and Setup

1. **Clone the project**

```bash
git clone https://github.com/bakytkann/final_backend.git
cd smartblog
```

2. **Create and activate a virtual environment**

```bash
python -m venv venv
source venv/bin/activate    # Linux/macOS
venv\Scripts\activate       # Windows
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Create a `.env` file**

```env
SECRET_KEY=your_secret_key
```

5. **Run the server**

```bash
python app.py
```