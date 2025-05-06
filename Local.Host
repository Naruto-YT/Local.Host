from flask import Flask, request

app = Flask(__name__)

@app.route('/')
def index():
    user_agent = request.headers.get('User-Agent')
    ip_address = request.remote_addr
    print(f"Visita desde: {user_agent}, IP: {ip_address}")
    return "Gracias por visitar. Tu información ha sido registrada."

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000)
