# 배열의 배열
- 바깥 배열 : 다른 배열들을 담을 배열
- 안쪽 배열 : 실제 값이 들어가는 배열

## 만드는 법
```c#
/* 바깥 배열 */
dataType[][] arrayName = new dataType[바깥 배열 원소 개수][];

string[][] classrooms = new string[3][];                      // 자깥 배열에 문자열 배열을 담을 공간을 3개 만든다

/* 안쪽 배열 */
바깥배열이름[색인] = new 자료형[안쪽 배열 요소 개수];

classrooms[0] = new string[3];
classrooms[1] = new string[2];
classrooms[2] = new string[5];

string[] studentNames = classrooms[0];                         // 바깥 배열의 첫번째 배열에 접근

/* 안쪽 배열 접근 */
바깥배열이름[바깥배열색인][안쪽배열색인] = 값;
classrooms[0][0] = "someName";

안쪽배열자료형 변수명 = 바깥배열이름[바깥배열색인];
string[] studentNames = classrooms[0];
studentNames[0] = "someName";
```

### Array.Copy(sourceArray, destinationArray, destinationArray.Length);
