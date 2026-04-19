# 🧪 Kubernetes Lab : StatefulSet with MySQL

This project demonstrates deploying a **MySQL database using a Kubernetes StatefulSet** with:

- 🔐 Secret for secure password management  
- 💾 Persistent Volume Claim (PVC) for data persistence  
- 🌐 Headless Service for stable networking  
- ⚙️ Tolerations for scheduling on tainted nodes  

---

---

## 🚀 Deployment Steps

### 1️⃣ Apply the configuration

```bash
kubectl apply -f secets.yaml
kubectl apply -f pvc.yaml
kubectl apply -f StatefulSet.yaml
kubectl apply -f HeadlessService.yaml
2️⃣ Verify resources
kubectl get pods
kubectl get svc
kubectl get pvc
3️⃣ Connect to MySQL
kubectl exec -it mysql-0 -- mysql -uroot -p
Enter your password when prompted.
```
✅ Sample Output
<img width="1446" height="592" alt="image" src="https://github.com/user-attachments/assets/17dfb59e-572a-4e61-bd5e-dffab80f3488" />

🛠️ Technologies Used
Kubernetes
Docker
MySQL 5.7
