FROM python:3.11-slim

# Diretório de trabalho
WORKDIR /app

# Cria usuário não-root
RUN useradd appuser

# Copia dependências
COPY requirements.txt .

# Instala dependências
RUN pip install --no-cache-dir -r requirements.txt

# Copia código
COPY app.py .

# Segurança: roda sem root
USER appuser

# Porta
EXPOSE 8080

# Start
CMD ["python", "app.py"]
