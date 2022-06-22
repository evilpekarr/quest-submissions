# quest-submissions

# Chapter 1 Day 1 
1. Blockchain is a database that stores, transmits, receives information. It is completely decentralized, that is, no one can manage it, it cannot be turned off (only if you turn off all the devices that support the blockchain, and there are thousands of such devices around the world). Blockchains can be different, perform different functions, but the main thing is that they can store information that cannot be deleted. The peculiarity of the blockchain is that it stores information in blocks, which has its own memory limit, upon reaching which a new block is created, and the old one is saved and creates a chain with others.

2. Smart contracts are programs that run if you need to perform some action if it is initiated. The conditions for the execution of smart contracts can be unlimited and it will only work successfully if all the conditions are met. Smart contracts are used to automate the execution of an agreement so that you can immediately be sure of the result without the participation of an intermediary and loss of time.

3. A script differs from a transaction in that a script is used to view information and can be run by anyone. A transaction changes data in the blockchain (adds, deletes) and it always costs some resources, often a transaction fee.

# Сhapter 1 Day 2

1. The 5 Cadence Programming Language Pillars is: Safety and Security, Clarity, Approachability, Developer Experience, Resource Oriented Programming.
2. This can help speed up the development process and improve the user experience in using the product.

# Сhapter 2 Day 1

1. 
![Screenshot_16](https://user-images.githubusercontent.com/101177946/174672705-6c07dc57-c316-4644-969e-b6205a97ccd4.jpg)

```
pub contract JacobTucker {
    pub let is: String

    init() {
        self.is = "the best!"
    }
}
```
2. 
![Screenshot_5](https://user-images.githubusercontent.com/101177946/174739558-a79fdd0a-d87c-48c5-9046-412560ed3414.jpg)

```
import JacobTucker from 0x03

pub fun main(): String {
    return JacobTucker.is
}
```

# Сhapter 2 Day 2

1. We would't call ```changeGreting``` in a script because it's a function. Script only reads and return information on the blochain.
2. It means that AuthAcc gives ability to read data in the account.|
3. ```prepare``` phase access information or data in your account while ```execute``` can't do that.  But it can call functions and do stuff to change the data on the blockchain.
4. 
![image](https://user-images.githubusercontent.com/101177946/175025277-05b50720-7ef7-4966-b6a8-7abb199dedec.png)

```
pub contract HelloWorld {

    pub var greeting: String
    pub var myNumber: Int

    pub fun changeGreeting(newGreeting: String) {
        self.greeting = newGreeting
    }
  
    pub fun updateMyNumber(newNumber: Int){
        self.myNumber = newNumber
    }

    init() {
        self.greeting = "Hello, World!"
        self.myNumber = 0
    }

}
```

![image](https://user-images.githubusercontent.com/101177946/175028564-6e8a6b11-cb9d-454f-9dd1-d21b24fa66ab.png)


```
import HelloWorld from 0x01

pub fun main(): Int {
    return HelloWorld.myNumber
}
```


