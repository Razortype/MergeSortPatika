# MergeSortPatika

## Questions
[16,21,11,8,12,22] -> Merge sort

1) Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2) Big-O gösterimini yazınız.

---

## Answers

### 1)

```
                                                             [16,21,11,8,12,22]

                                                        /                           \

                                                [16,21,11]                            [8,12,22]
                                    
                                              /            \                      /               \
                                    
                                         [16,21]           [11]                [8,12]              [22]

                                        /      \             /                 /    \               /

                                    [16]        [21]      [11]              [8]     [12]         [22]

                                      \          /         /                 \       /          /

                                         [16,21]        [11]                   [8,12]        [22]

                                            \          /                          \          /

                                             [11,16,21]                             [8,12,22]

                                                        \                        /

                                                            [8,11,12,16,21,22] 
```


### 2) 
    Her seferinde diziyi 2 ye bölüm sıraladığımız için O(log n)