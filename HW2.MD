## CShape.java        
abstract class CShape{
    protected String color;
    public void setColor(String str){
        color = str;
    }


    public abstract void show();
}

           
## CTriangle.java
class CTriangle extends CShape{
    double ca, cb, cc;
    public CTriangle(double a, double b, double c){
        ca=a;
        cb=b;
        cc=c;
    }
   
    public void show() {
       
        System.out.print("color="+color+"  ");
        System.out.print("area="+0.5*ca*cb);
    }
   
}

## app11.java
public class app11 {
   public static void main(String[] args) {
    CTriangle ct = new CTriangle(3, 4, 5);
    ct.setColor("red");
    ct.show();
}
}

---

# 專案管理

## 甘特圖
## 甘特圖
```mermaid
gantt
    title 甘特圖
　　研擬計畫     : a1 , 2023-10-03 , 1d
    任務分配     : a2 , after a1 , 4d
    取得硬體     : a3 , after a1 , 17d
    程式開發     : a4 , after a2 , 70d
    安裝硬體     : a5 , after a3 , 10d
    程式測試     : a6 , after a4 , 30d
    撰寫使用手冊  : a7 , after a5 , 25d
    轉換檔案     : a8 , after a5 , 20d
    系統測試     : a9 , after a6 , 25d
    使用者訓練   : a10 , after a7 a8 ,20d
    使用者測試   : a11 , after a9 a10 ,25d
```
## PERT/CPM圖
![999](999.png "999")
## 關鍵路徑
1-> 2-> 4-> 6-> 9-> 10-> 11
