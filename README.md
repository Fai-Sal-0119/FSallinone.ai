# FSallinone.ai
FS ALL IN ONE AI
gh repo clone Fai-Sal-0119/FSallinone.ai
cd FSallinone.ai
pip install -r requirements.txt
python main.py
http://localhost:8000 http://localhost:8000/docs http://localhost:8000/redoc # Health check
curl http://localhost:8000/health

# Prediction करें
curl -X POST http://localhost:8000/predict \
  -H "Content-Type: application/json" \
  -d '{"features": [1, 2, 3, 4, 5]}' git add .
git commit -m "Added AI features"
git push origin main
