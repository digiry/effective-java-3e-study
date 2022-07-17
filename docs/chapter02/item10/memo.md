# 10. equals 는 일반 규약을 지켜 재정의하라

### equals 동치관계 (equivalence relation) 일반 규약

반사성(reflexivity): null이 아닌 모든 참조 값 x에 대해 x.equals(x)는 true다

```
x == x , true다
```

대칭성(symmetry): null이 아닌 모든 참조 값 x, y에 대해, x.equals(y)가 true면 y.equals(x)도 true다

```
x == y, true 면 y == x, true 다
```

추이성(transitivity): null이 아닌 모든 참조 값 x,y,z에 대해 x.equals(y) 가 true이고 y.equals(z)도 true면 x.equals(z)도 true다

```
x == y true AND y == z true ==> x == z true
```

일관성(consistency): null이 아닌 모든 참조 값 x, y에 대해 x.equals(y)를 반복해서 호출하면 항상 true를 반환하거나 항상 false를 반환한다.

```
loop (true) {
    x == y true 
}
```

null 아님: null이 아닌 모든 참조 값 x 에 대해 x == null 은 false다

```
x == null false
```
