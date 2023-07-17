<script setup lang="ts">
let a: number = 88
console.log('🚀 ~ file: HelloWorld.vue:7 ~ a:', a)
let b = (): undefined => {
  console.log('★打印★', 77)
  return
}
console.log('🚀 ~ file: HelloWorld.vue:9 ~ b:', b)
const obj: boolean[] = []
console.log('🚀 ~ file: HelloWorld.vue:14 ~ obj:', obj)
let tbj: Array<boolean | number> = [false, 77]
console.log('🚀 ~ file: HelloWorld.vue:16 ~ tbj:', tbj)
let nn: unknown
nn = 88
if (typeof nn == 'number') {
  nn.toFixed(2)
}
console.log('🚀 ~ file: HelloWorld.vue:18 ~ nn:', nn)
let tt: { name: 'oo'; age: number } & { sex: boolean } = { name: 'oo', age: 178, sex: true }
console.log('🚀 ~ file: HelloWorld.vue:26 ~ tt:', tt)
interface kkx {
  name: string
  age: 18
}
const person: kkx = {
  name: 'kk',
  age: 18
}
console.log('🚀 ~ file: HelloWorld.vue:33 ~ person:', person)
interface IarrType {
  [index: number]: number | boolean
}
const arr: IarrType = [77, false]
console.log('🚀 ~ file: HelloWorld.vue:38 ~ arr:', arr)

interface Iobj {
  [key: string]: number
}
const obj2: Iobj = { name: 777, age: 88 }
console.log('🚀 ~ file: HelloWorld.vue:44 ~ obj2:', obj2)

interface iFunc {
  (a: string, b: number): void
}
const ucfunc: iFunc = (a, b) => {
  console.log('★打印★', a, b)
}
ucfunc('xming', 66)

type hhhh = string | number
let mm: hhhh = 44
console.log('🚀 ~ file: studyTest.vue:52 ~ mm:', mm)
type arrT = number[]
let rra: arrT = [0]
console.log('🚀 ~ file: studyTest.vue:54 ~ rra:', rra)

type objA = { name: string; age: number }
// type objB extends objA={
//     sex:boolean
// }
interface objB extends objA {
  sex: boolean
}
const objRes: objB = {
  name: 'kk',
  sex: true,
  age: 8
}
console.log('🚀 ~ file: studyTest.vue:68 ~ objRes:', objRes)
interface objC extends objB {
  height: number
}
const objRes2: objC = {
  name: 'kk',
  sex: true,
  age: 8,
  height: 184
}
console.log('🚀 ~ file: studyTest.vue:79 ~ objRes2:', objRes2)

type iFunc2 = {
  (a: string, b: number): void
}
const ucfunc2: iFunc2 = (a, b) => {
  console.log('★打印★', a, b)
}
ucfunc2('xming', 66)
</script>

<template>
  <div class="greetings"></div>
</template>

<style scoped></style>
