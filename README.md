# disjunctive-normal-form-monte-carlo
Please see the .jpg for the problem assignment. 

For this project we set out assuming that the possible universe of solutions was 8^15, and that hard solving 
using random sampling would be wildly insufficient. For example a sample of 10 million, would still be less 
than .00002% of our entire population. This meant that sample error could deviate exponentially per sample. 
Later on, we would realize that the professor had taken special care to make sure that this was not the case, 
but at the start it was quite a perplexing problem.

After some research, we discovered a graduate computer science lecture at MIT discussing sampling from such 
problem sets. Instead of hard solving for the values randomly, we designed an algorithm following the MIT lesson
that would sample from assignments that already were the solution for one clause. The idea was to sample only 
'the important space' non-uniformly to optimize the results of our algorithm.

Using random sampling as a base, we can see that our algorithm generated nearly identical solution for the problem.

과제를 수행하기에 앞서 저희 조는 문제의 풀이과정을 이해해보려고 하였습니다.
x의 값은 3 bits (000, 0001, 010, ..., 111) 이기에 0-7의 불규칙적 숫자로이루어져 있으며 총 x1-x15 변수로 구성되있습니다. 
때문에 가능한 전체의 해 (the possible universe of solutions) 는 8^15라고 생각할 수 있습니다.
하지만 random sampling을 통해 8^15양에 해당하는 모든 경우의 수를 구하고 분석하는건 어렵다고  생각하였습니다.
예를 들어 1000만 중 하나의 샘플링을 통해 답을 유도한다고 하여도 전체의 인구의 0.00002% 불과 합니다. 
이는 각 샘플에 해당하는 샘플 에러가 점점 더 기하급수적으로 증가함을 뜻합니다.
교수님께서 문제를 통해 도출하시려는 방법이 다른 방향일거라 생각하고 다른방법으로 문제에 접근해보려고 하였습니다.

MIT Computer Science Lecture 에서 힌트를 얻을 수 있었습니다. 
어렵게 불규칙적으로 여러 값들을 구하는 대신에, 하나의 "Clause"의 "Solution"인 "Assignments"들을 불규칙적으로
샘플링하는 알고리듬을 구현하여 답을 구하는 방식이었습니다.
바꾸어 말하면 중요하다고 생각되는 "Space"를 구분하여 "non-uniformly" 샘플링하는 최적화 방법 입니다.

랜덤샘플링을 기초로한 또다른 방법과 비교하였을때, 저희가 고안한 알고리듬이 비슷한 값을 도출해 내는것을 확인할 수 있었습니다.

