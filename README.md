
# Osteoarthritis Detection

An orthopaedist is a medical doctor specializing in diagnosing and treating disorders related to the skeletal system. Part of their job is to distinguish between a healthy person and a person with Osteoarthritis by looking at their knee X-ray images.

Osteoarthritis : Osteoarthritis, commonly known as wear-and-tear arthritis, is a condition in which the natural cushioning between joints -- cartilage -- wears away. When this happens, the bones of the joints rub more closely against one another with less of the shock-absorbing benefits of cartilage. The rubbing results in pain, swelling, stiffness, decreased ability to move, and sometimes the formation of bone spurs.


![Healthy joint](https://user-images.githubusercontent.com/97322648/156171347-879f1217-d3c4-44d7-8097-3085a50dc155.png)
**Healthy Knee Joint**

![osteoarthritis](https://user-images.githubusercontent.com/97322648/156171513-9d98472d-824b-4f2e-9057-1598603f1789.png)
**Osteoarthritis Joint**
## Dataset Description

The Dataset contains three folders  

* Test (845 images),  
* Train (2350 images),   
* Valid (641 images),  
Each of these folders has two folders  

* **Test**  
  * Normal  
  * Osteoarthritis  
  
* **Train**  
  * Normal  
  * Osteoarthritis  

* **Valid**  
  * Normal  
  * Osteoarthritis   

you can download the dataset [here](https://www.kaggle.com/vasanthgowdamk/osteoarthritis/download)


## Convolution Base (InceptionV3)

![image](https://user-images.githubusercontent.com/97322648/156175490-84fd844c-a9ed-46f3-a13f-f77a3e3224ef.png)


to import the model, run 

```bash
  from tensorflow.keras.applications import InceptionV3
```

## Deployment

To deploy this project run

```bash
  npm run deploy
```


## Result


![__results___18_0](https://user-images.githubusercontent.com/97322648/156173534-6add3f26-69ff-4ebc-8167-555623237f11.png)

The training stablized due to early stopping after achieving the following parametrs 

| Accuracy | in percentage |
| ------------- | ------------- |
| Training Accuracy| 94.08  |
| Validation Accuracy | 95.78  |

| Loss | in decimal  |
| ------------- | ------------- |
| Training loss| 0.1558  |
| Validation loss |  0.0981  |

The model trained for 46 epochs before early stopping conditions were met. 
