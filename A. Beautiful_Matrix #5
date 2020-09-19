"""
https://codeforces.com/contest/263/problem/A

5X5 Matrix
Solution:
Check how many times will it take
to bring 1 in the middle.

keep i+
and j+ until 2 2 

0 1 2 3 4 j
1
2 
3
4
i
-+ depending on the location of 1
till you get [2][2]
"""
def find_cord(index_number, number):
    """
    Returns The index in a 2D array.
    """
    for index, Value in enumerate(index_number):
        if number in Value:
            return (index, Value.index(number))

def solver(problem):
    steps = 0
    X_Coord = problem[0]
    Y_Coord = problem[1]

    while X_Coord != 2:
        if X_Coord == 2:
            break
        elif X_Coord > 2:
            X_Coord -= 1
            steps += 1
        elif X_Coord < 2:
            X_Coord += 1
            steps += 1

    while Y_Coord != 2:
        if Y_Coord == 2:
            break
        elif Y_Coord > 2:
            Y_Coord -= 1
            steps += 1
        elif Y_Coord < 2:
            Y_Coord += 1
            steps += 1

    return steps


if __name__ == '__main__':
    a = list()
    val = 1
    sentinel = []
    for i in range(5):
        a.append([int(j) for j in input().split()])
    Coordinates = find_cord(a, val)
    print(solver(Coordinates))
