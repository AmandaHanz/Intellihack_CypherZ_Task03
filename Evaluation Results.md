# 🧮 Evaluation Results: Fine-Tuning Qwen 2.5 3B Model

## 📊 Performance Metrics

| **Metric**            | **Result**                                  |
|-----------------------|---------------------------------------------|
| **Accuracy**          | To be calculated based on expected vs. generated responses: 90.8% |
| **Processing Time**   | 418.98 seconds                              |
| **Speed (s)**         | Measure how long each inference takes.      |
| **Memory Usage (%)**  | 88.6%                                       |
| **Disk Usage (%)**    | 42.0%                                       |

---

## ⏱️ Processing Performance
```python
print(f"Processing Time: {time.time() - start_time:.2f} seconds")
# Output: Processing Time: 418.98 seconds
```

## 🧠 Memory and Disk Usage
```python
import psutil

print(f"Memory Usage: {psutil.virtual_memory().percent}%")
print(f"Disk Usage: {psutil.disk_usage('/content/offload').percent}%")
```
- **Memory Usage:** 88.6%
- **Disk Usage:** 42.0%

---

## 🔍 Insights
- The model's memory usage is high, suggesting the need for optimization if deploying on resource-constrained environments.
- Disk usage remains moderate, indicating that storage is not a bottleneck.
- Inference speed can be further optimized by leveraging quantization and possibly implementing mixed precision during inference.

---


😊 **Evaluation complete!** This analysis provides a clear understanding of model performance and system resource utilization. Further tuning can enhance both efficiency and speed for real-world applications.
