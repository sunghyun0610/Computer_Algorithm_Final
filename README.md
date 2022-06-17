💻Computer Algorithm final-term assingment💻
<br> by 201901671 문성현
===========================================

## List
- **1.최적해(유전)알고리즘 원리 및 설명**
    - *1-1. P&Np(NP-hard)문제 소개*
    - *1-2. 용어 정리(사전지식) 및 유전알고리즘 원리 설명*
- **2.유전(Genetic) 알고리즘으로 코드(Python) 및 동작방식 설명**
- **3.회기식**
- **4.개선점과 하면서 새로 배우고 느낀 점**

## 1-1 **P&NP(NP-hard)문제 소개**
#### - P 문제는 결정 문제들 중에서 쉽게 풀리는 것을 모아 놓은 집합이다. 어떤 결정 문제가 주어졌을 때, 다항식(Polynomial) 시간 이내에 그 문제의 답을 YES와 NO 중의 하나로 계산해낼 수 있는 알고리즘이 존재하는 문제이다.     

#### -수업시간에 다루었던 **NP**(Non-deterministic Polynomial) 문제는 형식적으로는, 문제를 푸는 각 단계에서 여러가지의 가능성을 동시에 고려할 수 있는 비결정적 알고리즘(non-deterministic algorithm)으로 다항시간내에 문제를 해결할 수 있는 문제라고 정의한다. 즉,어떤 결정 문제의 답이 YES일 때, "그 문제의 답이 YES라는 것을 입증하는 힌트가 주어지면, 그 힌트를 사용해서 그 문제의 답이 정말로 YES라는 것을 다항식 시간 이내에 확인할 수 있는 문제가 바로 NP 문제에 해당된다."</br>
![Alt text](https://upload.wikimedia.org/wikipedia/commons/4/4a/Complexity_classes.png)
#### 사실 많은 컴퓨터공학자들은 절대로 P=NP일리가 없다고 믿고 있다. 왜냐하면, P=NP가 의미하는 바는, 만약 어떤 문제가 주어졌을 때, 그 문제의 답안을 쉽게 검산할 수 있다면, 그 문제 자체도 쉽게 풀 수 있다는, 너무나도 강력한 주장이기 때문이라고 수업시간에 배웠다.</br>


## 1-2. **용어 정리(사전지식) 및 유전알고리즘 원리 설명**
#### 유전 알고리즘은 생물체가 환경에 적응하면서 진화해가는 모습을 모방하여 ~~최적해~~를 찾아내는 검색 방법이다. 유전 알고리즘은 이론적으로 전역 최적점을 찾을 수 있으며, 수학적으로 명확하게 정의되지 않은 문제에도 적용할 수 있기 때문에 매우 유용하게 이용된다. 일반적으로 유전 알고리즘에 대해 알고리즘이라는 표현을 이용하지만, 유전 알고리즘은 특정한 문제를 풀기 위한 알고리즘이라기 보다는 **최적화 문제를 풀기 위한 방법론**에 가깝다. 즉, 모든 문제에 적용 가능한 하나의 알고리즘이나 소스 코드가 있는 것이 아니기 때문에 유전 알고리즘의 원리를 이해하고, 이를 자신이 원하는 문제에 적용할 수 있도록 하는 것이 중요하다고 생각한다.
### 용어정리
- **염색체(chromosome)**: 유전 알고리즘에서 하나의 해 (solution)를 표현한다. 즉 어떠한 문제의 해를 염색체로 치환한 것이다.
- **유전자(gene)**: 염색체를 구성하는 요소. 하나의 유전 정보를 나타낸다. 어떠한 염색체의 유전자가 [A B C]라면, 이 염색체에는 각각 A, B, C의 값을 갖는 3개의 gene이 존재한다.
- **자손 (offspring)**: 특정 시간 t에 존재했던 염색체들로부터 생성된 염색체를 t에 존재했던 염색체들의 자손이라고 한다. 자손은 이전 세대와 비슷한 유전 정보를 갖는다.
- **적합도 (fitness)**: 해당 문제에 대해 염색체가 표현하는 해가 얼마나 적합한지를 나타낸다.
유전학적으로는 염색체가 갖고 있는 고유값을 뜻한다.

### 알고리즘 구조
1. #### 초기 염새게의 집합 생성
2. #### 초기 염색체들에 대한 적합도 계산
3. #### 현재 염색체들로부터 자손들을 생성
4. #### 생성된 자손들의 적합도 계산
5. #### 종료 조건 판별
6. #### 종료 조건 거짓이면->3으로 이동하여 반복
#### =>즉 염색체집합에서 적합도가 가장 좋은 염색체를 선택하고, 선택된 해의 방향으로 검섹을 반복하면서 "최적해"를 찾아가는 구조이다.

### 연산 정의
#### 유전알고리즘은 앞서 언급했던 것처럼 자신이 원하는 문제에 적용할 수 있다.이를 위해선 총 5개의 연산을 정의하고 이해해야한다.
#### 1. 초기 염색체 생성 연산.
#### ->초기에는 이전 염색체가 존재하지 않기 때문에 선택된 염색체들로부터 자손을 생성할 수가 없다. 따라서, 초기 염색체를 생성하는 연산을 별도로 정의해야 한다. 
```
Random rand = new Random();
int[] chromosome = new int[SIZE_CHROMOSOME];
 
for(int i = 0; i < SIZE_CHROMOSOME; i++) {
    chromosome[i] = rand.nextInt(MAX_VAL_GENE);
}
```
#### 이와 같은 방법은 어떠한 규칙도 없이 임의의 값으로 염색체를 생성하는 것으로 이미 데이터가있는 경우에는 배열에 직접 입력하면 될것이다.

#### 2. 적합도를 계산하는 연산
#### -> 염색체에 표현된 정보를 기반으로 적합도를 계산하는 연산 

#### 3. 적합도를 기준으로 염색체 선택하는 연산
#### ->단순히 적합도가 가장 높은 두개를 선택하는 것은 다양성을이 크게 저하되기때문에 최적해를 찾기에는 부족할 것이다. 이를 보완하기 위해서 "룰렛 휠 선택" 방법을 사용한다.
#### P(ch.j)=f(Ch.j)/∑(i부터N까지)f(Ch.i)와 같은 수식
![Alt text](https://t1.daumcdn.net/cfile/tistory/260E9E3957DBBC7C15?download)
#### 즉 위의 수식을 이용하여 룰렛을 만들고 이를 이용하여 확률적으로 염색체를 선택하는 것이다.


#### 4.  선택된 염색체들로부터 자손을 생성하는 연산
#### 선택된 두개의 부모 염색체들로 부터 이제 자손 염색체를 생선하는 단계이다. 우리가 잘 알고있는 것처럼 부 유전자 + 모 유전자가 조합되어 =자손유전자가 된다. 이렇듯 염색체를 분할하는 행위를 "Crossover"라 하고 부 유전자와 모유전자를 분할하는 지점인 division point는 임의로 선택된다.
#### 5. ***돌연변이*** 연산
#### 드디어 유전알고리즘의 핵심이라고 할 수 있는 "돌연변이"를 계산할 차례이다. 돌연변이 요소를 추가하는 이유는 유전 알고리즘에서는 지역 최적점에 빠지는 문제를 해결하기 위해 새롭게 생성된 염색체에 확률적으로 돌연변이가 발생하도록 하는 것이다.(일반적으로 0.05%수준의 낮은 확률)
![Alt text](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=http%3A%2F%2Fcfile24.uf.tistory.com%2Fimage%2F236D374857DBC2AF2C3A50)
#### <br> 돌연변이는 두가지 종류가 있는데
- a)reverse: 하나의 유전자가 0->1 또는 1->0 으로 뒤집어지는 돌연변이
- b)exchange: 임의의 두개의 유전자가 서로 교환되는 돌연변이

## **2.유전(Genetic) 알고리즘을 이용한 TSP 코드(Python) 및 동작방식 설명**
#### 유전 알고리즘을 이용한 대표적인 문제인 TSP에대한 구현 코드 및 설명을 #(주석)을통해 설명해보았다.
#### 저의 주제는 스테픈커리의 골대와의 거리에 따른 슛성공률 변화 이지만 코드에 적용해 보는 것에 한계가 있어서 코드 설명은 TSP로 하였습니다!
#### 코드는 깃허브 레포지토리에도 있지만 readme파일에도 첨부하겠다.

```

import math
import random
import cv2#map이용하는 패키지


class City:# 한 도시의미
   def __init__(self, x=None, y=None):
      self.x = None#도시의 x좌표 지정
      self.y = None#도시의 y좌표 지정
      if x is not None:
         self.x = x
      else:
         self.x = int(random.random() * 200)
      if y is not None:
         self.y = y
      else:
         self.y = int(random.random() * 200)
   
   def getX(self):
      return self.x
   
   def getY(self):
      return self.y
   
   def distanceTo(self, city):#다른 도시간의 거리 값
      xDistance = abs(self.getX() - city.getX())
      yDistance = abs(self.getY() - city.getY())
      distance = math.sqrt( (xDistance*xDistance) + (yDistance*yDistance) )
      return distance
   
   def __repr__(self):
      return str(self.getX()) + ", " + str(self.getY())


class TourManager:#각 도시들을 연결한 경로
   destinationCities = []
   
   def addCity(self, city):
      self.destinationCities.append(city)
   
   def getCity(self, index):
      return self.destinationCities[index]
   
   def numberOfCities(self):
      return len(self.destinationCities)


class Tour:
   def __init__(self, tourmanager, tour=None):
      self.tourmanager = tourmanager
      self.tour = []
      self.fitness = 0.0#fitness=점수 , 거리와 반비례
      self.distance = 0
      if tour is not None:
         self.tour = tour
      else:
         for i in range(0, self.tourmanager.numberOfCities()):
            self.tour.append(None)
   
   def __len__(self):
      return len(self.tour)
   
   def __getitem__(self, index):
      return self.tour[index]
   
   def __setitem__(self, key, value):
      self.tour[key] = value
   
   def __repr__(self):
      geneString = "|"
      for i in range(0, self.tourSize()):
         geneString += str(self.getCity(i)) + "|"
      return geneString
   
   def generateIndividual(self):
      for cityIndex in range(0, self.tourmanager.numberOfCities()):
         self.setCity(cityIndex, self.tourmanager.getCity(cityIndex))
      random.shuffle(self.tour)
   
   def getCity(self, tourPosition):
      return self.tour[tourPosition]
   
   def setCity(self, tourPosition, city):
      self.tour[tourPosition] = city
      self.fitness = 0.0
      self.distance = 0
   
   def getFitness(self):
      if self.fitness == 0:
         self.fitness = 1/float(self.getDistance())# 거리가 짧을수록 점수가 높다!
      return self.fitness
   
   def getDistance(self):#tour의 총거리를 계산하는 함수
      if self.distance == 0:
         tourDistance = 0
         for cityIndex in range(0, self.tourSize()):
            fromCity = self.getCity(cityIndex)
            destinationCity = None
            if cityIndex+1 < self.tourSize():
               destinationCity = self.getCity(cityIndex+1)
            else:
               destinationCity = self.getCity(0)
            tourDistance += fromCity.distanceTo(destinationCity)
         self.distance = tourDistance
      return self.distance
   
   def tourSize(self):
      return len(self.tour)
   
   def containsCity(self, city):
      return city in self.tour

#유전 알고리즘 시작!
class Population:#tour들의 모임, 50개의 popultaion생성한다=50개의 투어가 있다. 여러가지 투어 거리들을 계산하고 fitness(점수)가 높은것들을 mutate(돌연변이)+crossover해서 최적해 찾는 과정
   def __init__(self, tourmanager, populationSize, initialise):
      self.tours = []
      for i in range(0, populationSize):
         self.tours.append(None)
      
      if initialise:
         for i in range(0, populationSize):
            newTour = Tour(tourmanager)
            newTour.generateIndividual()
            self.saveTour(i, newTour)
      
   def __setitem__(self, key, value):
      self.tours[key] = value
   
   def __getitem__(self, index):
      return self.tours[index]
   
   def saveTour(self, index, tour):
      self.tours[index] = tour
   
   def getTour(self, index):
      return self.tours[index]
   
   def getFittest(self):
      fittest = self.tours[0]
      for i in range(0, self.populationSize()):
         if fittest.getFitness() <= self.getTour(i).getFitness():
            fittest = self.getTour(i)
      return fittest
   
   def populationSize(self):
      return len(self.tours)


class GA:#유전 알고리즘의 핵심
   def __init__(self, tourmanager):
      self.tourmanager = tourmanager
      self.mutationRate = 0.015#돌연변이 일어날 확률
      self.tournamentSize = 5
      self.elitism = True
   
   def evolvePopulation(self, pop):#진화과정
      newPopulation = Population(self.tourmanager, pop.populationSize(), False)
      elitismOffset = 0
      if self.elitism:
         newPopulation.saveTour(0, pop.getFittest())
         elitismOffset = 1
      
      for i in range(elitismOffset, newPopulation.populationSize()):
         parent1 = self.tournamentSelection(pop)
         parent2 = self.tournamentSelection(pop)
         child = self.crossover(parent1, parent2)
         newPopulation.saveTour(i, child)
      
      for i in range(elitismOffset, newPopulation.populationSize()):
         self.mutate(newPopulation.getTour(i))
      
      return newPopulation
   
   def crossover(self, parent1, parent2):#crossover
      child = Tour(self.tourmanager)
      
      startPos = int(random.random() * parent1.tourSize())
      endPos = int(random.random() * parent1.tourSize())
      
      for i in range(0, child.tourSize()):
         if startPos < endPos and i > startPos and i < endPos:
            child.setCity(i, parent1.getCity(i))
         elif startPos > endPos:
            if not (i < startPos and i > endPos):
               child.setCity(i, parent1.getCity(i))
      
      for i in range(0, parent2.tourSize()):
         if not child.containsCity(parent2.getCity(i)):
            for ii in range(0, child.tourSize()):
               if child.getCity(ii) == None:
                  child.setCity(ii, parent2.getCity(i))
                  break
      
      return child
   
   def mutate(self, tour):#변이과정
      for tourPos1 in range(0, tour.tourSize()):
         if random.random() < self.mutationRate:
            tourPos2 = int(tour.tourSize() * random.random())
            
            city1 = tour.getCity(tourPos1)
            city2 = tour.getCity(tourPos2)
            
            tour.setCity(tourPos2, city1)
            tour.setCity(tourPos1, city2)
   
   def tournamentSelection(self, pop):
      tournament = Population(self.tourmanager, self.tournamentSize, False)
      for i in range(0, self.tournamentSize):
         randomId = int(random.random() * pop.populationSize())
         tournament.saveTour(i, pop.getTour(randomId))
      fittest = tournament.getFittest()
      return fittest



if __name__ == '__main__':
    n_cities = 20
    population_size = 50
    n_generations = 100

    random.seed(100)

    # Load the map
    map_original = cv2.imread('map.jpg')

    # Setup cities and tour
    tourmanager = TourManager()

    for i in range(n_cities):
        x = random.randint(200, 800)
        y = random.randint(200, 800)

        tourmanager.addCity(City(x=x, y=y))
        cv2.circle(map_original, center=(x, y), radius=10, color=(0, 0, 255), thickness=-1, lineType=cv2.LINE_AA)

    cv2.imshow('map', map_original)
    cv2.waitKey(0)

    # Initialize population
    pop = Population(tourmanager, populationSize=population_size, initialise=True)
    print("Initial distance: " + str(pop.getFittest().getDistance()))

    # Evolve population
    ga = GA(tourmanager)

    for i in range(n_generations):
        pop = ga.evolvePopulation(pop)

        fittest = pop.getFittest()

        map_result = map_original.copy()

        for j in range(1, n_cities):
            cv2.line(
                map_result,
                pt1=(fittest[j-1].x, fittest[j-1].y),
                pt2=(fittest[j].x, fittest[j].y),
                color=(255, 0, 0),
                thickness=3,
                lineType=cv2.LINE_AA
            )

        cv2.putText(map_result, org=(10, 25), text='Generation: %d' % (i+1), fontFace=cv2.FONT_HERSHEY_SIMPLEX, fontScale=0.7, color=0, thickness=1, lineType=cv2.LINE_AA)
        cv2.putText(map_result, org=(10, 50), text='Distance: %.2fkm' % fittest.getDistance(), fontFace=cv2.FONT_HERSHEY_SIMPLEX, fontScale=0.7, color=0, thickness=1, lineType=cv2.LINE_AA)
        cv2.imshow('map', map_result)
        if cv2.waitKey(100) == ord('q'):
            break

    # Print final results
    print("Finished")
    print("Final distance: " + str(pop.getFittest().getDistance()))
    print("Solution:")
    print(pop.getFittest())

    cv2.waitKey(0)
```
#### 유전 알고리즘에서 돌연변이는 지역 최적점에 빠지는 문제를 해결하기 위해 새롭게 생성된 염색체에 확률적으로 돌연변이가 발생하도록 하는 것이다.(일반적으로 0.05%수준의 낮은 확률)
- 돌연변이 확률이 너무 높을 경우: 너무 많은 변이가 발생해 시간복잡도가 증가한다
- 돌연변이 확률이 너무 낮을 경우: 모든 경우의 수를 다 고려하지 못하여 최적해를 구할 확률이 낮아진다. 
#### 라고  정리할 수 있겠습니다.
#### 여기까지 유전알고리즘에 대해 알아보았고 이제 제가 정한 주제를 소개하겠습니다.
## **3.회기식**
# Topic : 클릭횟수에 따른 광고 노출 빈도 데이터 그래프와 회기식
/*회귀식이란? Y=f(x)에서 한쪽의 변수에서 다른쪽의 변수 값을 예측하기 위한 방정식을 회귀식이라 하고 Y를 종속변수, X를 독립 변수라고 한다.*/
![Alt text](https://github.com/sunghyun0610/Computer_Algorithm_Final/blob/main/%ED%9A%8C%EA%B7%80%EC%8B%9D%20%EA%B7%B8%EB%9E%98%ED%94%84%20%EC%98%88.png?raw=true)
#### 클릭횟수에 따른 광고 노출 빈도 데이터 그래프와 회기식
![Alt text](https://github.com/sunghyun0610/Computer_Algorithm_Final/blob/main/%EA%B4%91%EA%B3%A0-%ED%81%B4%EB%A6%AD%20%EB%8D%B0%EC%9D%B4%ED%84%B0.png?raw=true)
![Alt text](https://github.com/sunghyun0610/Computer_Algorithm_Final/blob/main/%ED%9A%8C%EA%B7%80%EC%8B%9D.png?raw=true)

# Topic : 거리에 따른 스테픈 커리의 슛 성공률 변화를 매달 주기로 알아보고 회기식을 통해 오차를 최소화되게 다음달 예측.
