---
layout: post
title: "Java LinkedList, Stack, Queue 구현"
date: 2021-01-25 01:00:00 +0900
categories: Java DataStructure
---

---
## 1. 코드
LinkedList를 구현하였다. Stack, Queue 또한 구현한 LinkedList 기반이다.
###### Github : <a href="https://github.com/sanguk2/ExampleCode/tree/main/list/src">ExampleCode Repository</a>

---
## 2. LinkedList
데이터와 다음 데이터의 주소를 가지는 노드를 활용해 서로 연결시킨 자료구조이다. 노드들은 다음 노드의 주소값을 가지고 있으며, 이 주소값을 통해 데이터에 각각의 접근할 수 있다.

<img alt="linked-list-concept" src="https://user-images.githubusercontent.com/51690528/105637139-4253ad80-5eaf-11eb-8ccf-d2cd1765c4a0.png">

출처 : <a href="https://www.programiz.com/dsa/linked-list">LinkedList Data Structure</a>

### 2. 데이터의 삽입
##### 1. 새로운 노드를 생성한다. 이후 preNode의 주소에 저장되어 있던 다음 노드의 주소값을 새로 만든 노드에 저장한다.
![linked_list_insert_1](https://user-images.githubusercontent.com/51690528/105637755-66fd5480-5eb2-11eb-8409-90714b4ece18.jpg)

##### 2. preNode의 주소에 새로 생성한 노드의 주소값을 저장한다.
![linked_list_insert_2](https://user-images.githubusercontent.com/51690528/105637756-6795eb00-5eb2-11eb-87d6-20c335341d5e.jpg)

### 3. 데이터의 삭제
![linked_list_remove_1](https://user-images.githubusercontent.com/51690528/105638207-c52b3700-5eb4-11eb-8f89-8d7e25aba57f.jpg)

##### 1. 삭제하고자 하는 노드의 주소에 저장되어 있던 값을 이전 노드의 주소에 저장한다.
![linked_list_remove_2](https://user-images.githubusercontent.com/51690528/105638208-c5c3cd80-5eb4-11eb-85d5-790acd7ec605.jpg)

---
## 3. Stack
한 쪽 끝에서만 자료를 넣거나 뺄 수 있는 선형 자료구조(LIFO - Last In First Out)이다. 가장 나중에 삽입된 데이터가 먼저 제거된다.

<img alt="stack" src="https://user-images.githubusercontent.com/51690528/105637221-a70f0800-5eaf-11eb-96db-238c17d6d9b3.png">

출처 : <a href="https://www.programiz.com/dsa/stack">Stack Data Structure</a>

### 2. 데이터의 삽입
##### 1. 새로운 노드를 생성한다. 새로 생성한 노드의 주소에 top 노드의 주소값을 저장한다.
##### 2. 새로운 노드를 top 노드로 변경한다.
![linked_list_stack_push](https://user-images.githubusercontent.com/51690528/105638895-ab8bee80-5eb8-11eb-803d-df46d742ac73.jpg)


### 3. 데이터의 삭제
##### 1. top 노드를 삭제하고자 하는 노드의 다음 노드로 변경한다.
![linked_list_stack_pop](https://user-images.githubusercontent.com/51690528/105638892-aa5ac180-5eb8-11eb-83c4-d1ff33498384.jpg)

---
## 4. Queue
먼저 집어 넣은 데이터가 먼저 나오는 FIFO(First In First Out)구조로 저장하는 자료구조이다. 가장 나중에 삽입된 데이터가 가장 나중에 제거된다.

<img alt="queue" src="https://user-images.githubusercontent.com/51690528/105639155-f6f2cc80-5eb9-11eb-9578-4843c001cce4.png">

출처 : <a href="https://www.programiz.com/dsa/queue">Queue Data Structure</a>

### 2. 데이터의 삽입
##### 1. 새로운 노드를 생성한다.
![linked_list_queue_enqueue_1](https://user-images.githubusercontent.com/51690528/105639479-ee02fa80-5ebb-11eb-8311-25d2aeb82e3b.jpg)

##### 2. rear 노드에 새로 만든 노드의 주소를 저장한다. 그 후 새로운 노드를 rear로 변경한다.
![linked_list_queue_enqueue_2](https://user-images.githubusercontent.com/51690528/105639481-ef342780-5ebb-11eb-860b-a5b744e3a7e7.jpg)

### 3. 데이터의 삭제
![linked_list_queue_enqueue_2](https://user-images.githubusercontent.com/51690528/105639481-ef342780-5ebb-11eb-860b-a5b744e3a7e7.jpg)

##### 1. head 노드를 삭제하고자 하는 노드에서 그 다음 노드로 변경한다.
![linked_list_queue_dequeue](https://user-images.githubusercontent.com/51690528/105639482-ef342780-5ebb-11eb-8965-a39c854c68f2.jpg)

---

## 5. 참고할 점
자바의 경우, 참조가 해제된 스택의 데이터를 자동으로 해제해주는 가비지 컬렉터 존재하므로 메모리의 할당이나 해제를 신경쓰지 않아도 괜찮다. 하지만, 메모리의 제어 권한이 개발자에게 존재하는 C 등의 언어로 구현할 경우 메모리의 할당, 해제에 대해 구현할 필요가 있다. <br>
또, 자바에서는 이러한 자료구조가 이미 구현되어 있다. Collection 중 LinkedList, Stack 등이 그것이다. 실제 사용할 때는 직접 구현이 아닌 해당 Collection을 사용하는 것이 권장된다.

---
### ▶ Reference
- <a href="https://www.programiz.com/dsa/linked-list">LinkedList Data Structure</a>
- <a href="https://www.programiz.com/dsa/stack">Stack Data Structure</a>
- <a href="https://www.programiz.com/dsa/queue">Queue Data Structure</a>
- 남궁성, 『자바의 정석』, 도우출판

---
