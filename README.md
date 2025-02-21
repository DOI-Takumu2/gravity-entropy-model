# グラビティ－エントロピーモデル［gravity-entropy-model］

## 概要
本アプリケーションは、**グラビティモデル** と **エントロピー最大化モデル** の流動分析を実装できます。  
Excelデータをアップロードすることで分析を実行できます。

## 製作者
- **土居拓務（Takumu Doi）**  
---

## **機能**
✅ **Excelデータをアップロードし、流動分析を実施**  
✅ **グラビティモデルとエントロピー最大化モデルのいずれかを選択**  
✅ **統計指標 (MSE, RMSE, MAE, R²) を算出**  
✅ **結果をExcelファイルとしてダウンロード可能**  
---

### **2. Excelファイルをアップロード**
- 「ファイルをアップロード」ボタンをクリックし、Excelデータを選択
- フォーマットの例:
  
| Origin | Destination | Distance | Population_Origin | Population_Destination | Flow |
|--------|------------|----------|------------------|--------------------|------|
| A      | X          | 10       | 1000             | 800                | 80   |
| A      | Y          | 15       | 1000             | 1200               | 60   |
| B      | Z          | 20       | 1500             | 1000               | 50   |

### **3. 分析モデルを選択**
- **グラビティモデル:** 対数線形回帰を用いた流動予測
- **エントロピー最大化モデル:** シングリーコンストレインドモデルによる最適化

### **4. 結果を確認**
- 結果を画面上に表示
- 統計指標（MSE, RMSE, MAE, R²）を確認可能

### **5. Excelファイルをダウンロード**
- 解析結果をExcel形式 (`.xlsx`) でダウンロード可能

---

## **ローカル環境での実行**
### **1. 必要なライブラリをインストール**
ターミナルで以下を実行：
```bash
pip install -r requirements.txt

