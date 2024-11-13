<template>
  <div>
    <div class="flex w-auto lg:mx-56 mx-20 mt-12 mb-10">
      <div class="w-60 lg:w-96 flex-col">
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
            {{ floarNumber }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 8 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 7 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 6 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 5 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloar('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 bg-white" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
            {{ floarNumber8 }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars8(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 7 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars8(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 6 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars8(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 5 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars8(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars8(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars8(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars8(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars8(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor88 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars8('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
            {{ floarNumber7 }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars7(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars7(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 6 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars7(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 5 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars7(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars7(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars7(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars7(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars7(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor77 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars7('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
            {{ floarNumber6 }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars6(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars6(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars6(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 5 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars6(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars6(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars6(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars6(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars6(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor66 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars6('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
            {{ floarNumber5 }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor55 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars5(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor55 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars5(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor55 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars5(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor55 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars5(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                             :style="{
                backgroundColor: changeColor55 == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars5(4)"
             
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                           :style="{
                backgroundColor: changeColor55 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars5(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                           :style="{
                backgroundColor: changeColor55 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars5(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                           :style="{
                backgroundColor: changeColor55 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars5(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                           :style="{
                backgroundColor: changeColor55 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars5('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
            {{ floarNumber4 }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor44 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars4(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor44 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars4(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor44 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars4(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor44 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars4(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor44 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars4(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                           :style="{
                backgroundColor: changeColor44 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars4(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                            :style="{
                backgroundColor: changeColor44 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars4(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                            :style="{
                backgroundColor: changeColor44 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars4(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                            :style="{
                backgroundColor: changeColor44 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars4('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
            {{ floarNumber3 }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor33 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars3(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor33 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars3(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor33 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars3(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor33 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars3(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor33 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars3(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor33 == 4 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars3(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                            :style="{
                backgroundColor: changeColor33 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars3(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                            :style="{
                backgroundColor: changeColor33 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars3(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                            :style="{
                backgroundColor: changeColor33 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars3('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-3xl text-black"
          >
            {{ floarNumber2 }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor22 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars2(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor22 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars2(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor22 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars2(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor22 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars2(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor22 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars2(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor22 == 4 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars2(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor22 == 3 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars2(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                                  :style="{
                backgroundColor: changeColor22 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars2(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                                          :style="{
                backgroundColor: changeColor22 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars2('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-2 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
            {{ floarNumber1 }}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                 :style="{
                backgroundColor: changeColor11 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars1(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor11 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars1(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor11 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars1(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor11 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars1(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor11 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars1(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor11 == 4 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars1(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor11 == 3 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars1(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColor11 == 2 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars1(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                                           :style="{
                backgroundColor: changeColor11 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloars1('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 ml-3 text-center text-4xl text-black"
          >
             {{floarNumber0}}
          </div>
          <div class="flex row mt-16 text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor00 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor00 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColor00 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor00 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor00 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor00 == 4 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor00 == 3 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor00 == 2 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColor00 == 1 ? 'green' : 'gray-500',
              }"
              @click="increaseFloars0(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
      </div>
      <div class="bg-white lg:w-40 w-40">
        <div class="h-1/6 border-t-8 border-gray-300">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
              {{ number9 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
              {{ number9 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer"
              @click="goingUp"
              :style="{
                backgroundColor: changeColorM ? 'green' : 'aliceblue',
                color: changeColorM ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer"
              @click="goingDown"
              :style="{
                backgroundColor: changeColorD ? 'green' : 'aliceblue',
                color: changeColorD ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
              {{ number8 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
              {{ number8 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer"
              @click="goingUp8"
              :style="{
                backgroundColor: changeColorM8 ? 'green' : 'aliceblue',
                color: changeColorM8 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer"
              @click="goingDown8"
              :style="{
                backgroundColor: changeColorD8 ? 'green' : 'aliceblue',
                color: changeColorD8 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
              {{ number7 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
              {{ number7 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer"
              @click="goingUp7"
              :style="{
                backgroundColor: changeColorM7 ? 'green' : 'aliceblue',
                color: changeColorM7 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer"
              @click="goingDown7"
              :style="{
                backgroundColor: changeColorD7 ? 'green' : 'aliceblue',
                color: changeColorD7 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
              {{ number6 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
              {{ number6 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer"
              @click="goingUp6"
              :style="{
                backgroundColor: changeColorM6 ? 'green' : 'aliceblue',
                color: changeColorM6 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer"
              @click="goingDown6"
              :style="{
                backgroundColor: changeColorD6 ? 'green' : 'aliceblue',
                color: changeColorD6 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
              {{ number5 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
              {{ number5 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer"  @click="goingUp5"
              :style="{
                backgroundColor: changeColorM5 ? 'green' : 'aliceblue',
                color: changeColorM5 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer"  @click="goingDown5"
              :style="{
                backgroundColor: changeColorD5 ? 'green' : 'aliceblue',
                color: changeColorD5 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
              {{ number4 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
              {{ number4 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer"  @click="goingUp4"
              :style="{
                backgroundColor: changeColorM4 ? 'green' : 'aliceblue',
                color: changeColorM4 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer" @click="goingDown4"
              :style="{
                backgroundColor: changeColorD4 ? 'green' : 'aliceblue',
                color: changeColorD4 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
               {{ number3 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
               {{ number3 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer"  @click="goingUp3"
              :style="{
                backgroundColor: changeColorM3 ? 'green' : 'aliceblue',
                color: changeColorM3 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer"  @click="goingDown3"
              :style="{
                backgroundColor: changeColorD3 ? 'green' : 'aliceblue',
                color: changeColorD3 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
              {{ number2 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
              {{ number2 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer" @click="goingUp2"
              :style="{
                backgroundColor: changeColorM2 ? 'green' : 'aliceblue',
                color: changeColorM2 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer" @click="goingDown2"
              :style="{
                backgroundColor: changeColorD2 ? 'green' : 'aliceblue',
                color: changeColorD2 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
               {{ number1 }}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
               {{ number1 }}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer" 
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer" @click="goingDown1"
              :style="{
                backgroundColor: changeColorD1 ? 'green' : 'aliceblue',
                color: changeColorD1 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
        <div class="h-1/6 border-t-8 border-gray-300 mt-4">
          <div class="flex">
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold border-r-2"
            >
             {{number0}}
            </div>
            <div
              class="bg-gray-100 w-36 h-24 text-4xl pl-5 text-red-400 font-bold"
            >
              {{number0}}
            </div>
          </div>
          <div class="ml-14 flex-col text-3xl mt-1 mb-1">
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-green-300 border-4 mb-2 cursor-pointer"
            >
              <i class="fa-solid fa-chevron-up"></i>
            </div>
            <div
              class="btn bg-gray-200 w-14 h-14 rounded-full pl-3 pt-1 border-red-300 border-4 mb-2 cursor-pointer" @click="goingDown0"
              :style="{
                backgroundColor: changeColorD0 ? 'green' : 'aliceblue',
                color: changeColorD0 ? 'white' : 'black',
              }"
            >
              <i class="fa-solid fa-chevron-down"></i>
            </div>
          </div>
        </div>
      </div>
      <div class="lg:w-96 flex-col w-60">
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 text-center text-4xl text-black ml-5"
          >
            {{ floarNumberr }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 8 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 7 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 6 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 5 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarr('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 ml-5 text-center text-4xl text-black"
          >
            {{ floarNumberr8 }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs8(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 7 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs8(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 6 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs8(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 5 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs8(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs8(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs8(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs8(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs8(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr88 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs8('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 ml-5 text-center text-4xl text-black"
          >
            {{ floarNumberr7 }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs7(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs7(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 6 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs7(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 5 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs7(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs7(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs7(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs7(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs7(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr77 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs7('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 ml-5 text-center text-4xl text-black"
          >
            {{ floarNumberr6 }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs6(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs6(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs6(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 5 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs6(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs6(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs6(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs6(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs6(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr66 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs6('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 text-center text-4xl ml-5 text-black"
          >
            {{ floarNumberr5 }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr55 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs5(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2" 
                  :style="{
                backgroundColor: changeColorr55 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs5(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                  :style="{
                backgroundColor: changeColorr55 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs5(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44 ">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                  :style="{
                backgroundColor: changeColorr55 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs5(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr55 == 4 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs5(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2" :style="{
                backgroundColor: changeColorr55 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs5(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr55 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs5(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr55 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs5(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr55 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs5('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 ml-5 text-center text-4xl text-black"
          >
            {{ floarNumberr4 }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                  :style="{
                backgroundColor: changeColorr44 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs4(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr44 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs4(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr44 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs4(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr44 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs4(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr44 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs4(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"    :style="{
                backgroundColor: changeColorr44 == 3 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs4(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"  :style="{
                backgroundColor: changeColorr44 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs4(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2" 
               :style="{
                backgroundColor: changeColorr44 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs4(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"  :style="{
                backgroundColor: changeColorr44 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs4('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 ml-5 text-center text-4xl text-black"
          >
            {{ floarNumberr3 }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr33 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs3(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2" 
               :style="{
                backgroundColor: changeColorr33 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs3(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr33 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs3(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr33 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs3(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2" 
               :style="{
                backgroundColor: changeColorr33 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs3(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2" 
               :style="{
                backgroundColor: changeColorr33 == 4 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs3(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr33 == 2 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs3(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr33 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs3(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr33 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs3('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 ml-5 text-center text-4xl text-black"
          >
            {{ floarNumberr2 }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr22 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs2(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr22 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs2(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr22 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs2(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr22 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs2(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr22 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs2(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr22 == 4 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs2(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              :style="{
                backgroundColor: changeColorr22 == 3 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs2(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
              
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr22 == 1 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs2(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr22 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs2('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 ml-5 text-center text-4xl text-black"
          >
             {{ floarNumberr1 }}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
               :style="{
                backgroundColor: changeColorr11 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs1(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColorr11 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs1(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColorr11 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs1(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColorr11 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs1(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColorr11 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs1(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColorr11 == 4 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs1(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:only:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColorr11 == 3 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs1(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                :style="{
                backgroundColor: changeColorr11 == 2 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs1(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                  :style="{
                backgroundColor: changeColorr11 == 0 ? 'green' : 'gray-500',
              }"
              @click="decreaseFloarrs1('G')"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
        <div
          class="bg-gray-200 border-b-8 h-1/6 border-l-8 border-gray-400 border-r-8 border-t-8 flex-col"
        >
          <div
            class="bg-white border-4 border-green-400 w-44 mt-20 h-20 lg:ml-44 ml-5 text-center text-4xl text-black"
          >
            {{floarNumberr0}}
          </div>
          <div class="flex row mt-16 text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                 :style="{
                backgroundColor: changeColorr10 == 9 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(9)"
            >
              9
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                   :style="{
                backgroundColor: changeColorr10 == 8 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(8)"
            >
              8
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                   :style="{
                backgroundColor: changeColorr10 == 7 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(7)"
            >
              7
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                   :style="{
                backgroundColor: changeColorr10 == 6 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(6)"
            >
              6
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                   :style="{
                backgroundColor: changeColorr10 == 5 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(5)"
            >
              5
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                   :style="{
                backgroundColor: changeColorr10 == 4 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(4)"
            >
              4
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                   :style="{
                backgroundColor: changeColorr10 == 3 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(3)"
            >
              3
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                   :style="{
                backgroundColor: changeColorr10 == 2 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(2)"
            >
              2
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
                   :style="{
                backgroundColor: changeColorr10 == 1 ? 'green' : 'gray-500',
              }"
              @click="increaseFloarrs0(1)"
            >
              1
            </button>
          </div>
          <div class="text-3xl lg:ml-44">
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-right mr-1"></i
              ><i class="fa-solid fa-caret-left"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              <i class="fa-solid fa-caret-left"></i
              ><i class="fa-solid fa-caret-right"></i>
            </button>
            <button
              class="bg-gray-500 border-4 shadow-lg border-green-200 w-12 h-12 text-white rounded-full mt-5 ml-2"
            >
              G
            </button>
          </div>
        </div>
        <hr class="text-white border-8 b" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      number9: 1,
      floarNumber: 9,
      floarNumberr: 9,
      changeColorD: false,
      changeColorM: false,
      changeColor: 10,
      changeColorr: 10,
      number8: 1,
      floarNumber8: 8,
      floarNumberr8: 8,
      changeColorM8: false,
      changeColorD8: false,
      changeColor88: 10,
      changeColorr88: 10,
      number7: 1,
      floarNumber7: 7,
      floarNumberr7: 7,
      changeColorD7: false,
      changeColorM7: false,
      changeColor77: 10,
      changeColorr77: 10,
      number6: 1,
      floarNumber6: 6,
      floarNumberr6: 6, 
      changeColorD6: false,
      changeColorM6: false,
      changeColor66: 10,
      changeColorr66: 10,
      number5: 1,
      floarNumber5: 5,
      floarNumberr5: 5,
      changeColorD5: false,
      changeColorM5: false,
      changeColor55: 10,
      changeColorr55: 10,
       number4: 1,
      floarNumber4: 4,
      floarNumberr4: 4,
      changeColorD4: false,
      changeColorM4: false,
      changeColor44: 10,
      changeColorr44: 10,
      number3: 1,
      floarNumber3: 3,
      floarNumberr3: 3,
      changeColorD3: false,
      changeColorM3: false,
      changeColor33: 10,
      changeColorr33: 10,
      number2: 1,
      floarNumber2: 2,
      floarNumberr2: 2,
      changeColorD2: false,
      changeColorM2: false,
      changeColor22: 10,
      changeColorr22: 10,
      number1: 9,
      floarNumber1: 1,
      floarNumberr1: 1,
      changeColorD1: false,
      changeColorM1: false,
      changeColor11: 10,
      changeColorr11: 10,
      number0: 9,
      floarNumber0: 'G',
      floarNumberr0: 'G',
      changeColorD0: false,
      changeColorM0: false,
      changeColor00: 10,
      changeColorr10: 10,
    };
  },
  methods: {
      increaseLift0() {
      this.number0--;
    },

    decreaseLift0() {
      this.number0++;
    },
    decreaseFloarrs0(value) {
      this.floarNumberr0 = 1;
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr0();
        if (this.floarNumberr0 == value) {
          this.changeColorr10 = value;
          clearInterval(intervalID2);
          this.floarNumberr0 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr0 == 0) {
          this.changeColorr10 = 0;
          clearInterval(intervalID2);
          this.floarNumberr0 = "G";
        }
      }, 1000);
    },
    goingUp0() {
      this.changeColorD0 = false;
      this.number0 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift0();
        if (this.number0 == 1) {
          clearInterval(intervalID);
          this.changeColorM0 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    goingDown0() {
      this.changeColorM0 = false;
      let intervalID = setInterval(() => {
        this.increaseLift0();
        if (this.number0 === 0) {
          clearInterval(intervalID);
          this.changeColorD0 = true;
          console.log("Interval Cleared");
          this.number0 = "G";
        }
      }, 1000);
    },
    decreaseFloar0() {
      this.floarNumber0 = 0
      this.floarNumber0--;
    },

    decreaseFloarr0() {
      this.floarNumberr0--;
    },
      increaseFloars0(value) {
         this.floarNumber0 = 1
      let intervalID8 = setInterval(() => {
        this.increaseFloar0();
        if (this.floarNumber0 == value) {
          this.changeColor00 = value;
          clearInterval(intervalID8);
          this.floarNumber0 == value;
        }
      }, 1000);
    },
      increaseFloarr0() {
      this.floarNumberr0++;
    },
    increaseFloar0() {
      
      this.floarNumber0++;
    },
      increaseFloarrs0(value) {
         this.floarNumberr0 = 1;
      let intervalID8 = setInterval(() => {
        this.increaseFloarr0();
        if (this.floarNumberr0 == value) {
          this.changeColorr10 = value;
          clearInterval(intervalID8);
          this.floarNumberr0 == value;
        }
      }, 1000);
    },
   
      increaseLift1() {
      this.number1--;
    },

    decreaseLift1() {
      this.number1++;
    },
    decreaseFloarrs1(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr1();
        if (this.floarNumberr1 == value) {
          this.changeColorr11 = value;
          clearInterval(intervalID2);
          this.floarNumberr1 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr1 == 0) {
          this.changeColorr11 = 0;
          clearInterval(intervalID2);
          this.floarNumberr1 = "G";
        }
      }, 1000);
    },
    goingUp1() {
      this.changeColorD1 = false;
      this.number1 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift1();
        if (this.number1 == 1) {
          clearInterval(intervalID);
          this.changeColorM1 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    goingDown1() {
      this.changeColorM1 = false;
      let intervalID = setInterval(() => {
        this.increaseLift1();
        if (this.number1 === 1) {
          clearInterval(intervalID);
          this.changeColorD1 = true;
          console.log("Interval Cleared");
          this.number1 = 1;
        }
      }, 1000);
    },
    decreaseFloar1() {
      this.floarNumber1--;
    },

    decreaseFloarr1() {
      this.floarNumberr1--;
    },
     increaseFloars1(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloar1();
        if (this.floarNumber1 == value) {
          this.changeColor11 = value;
          clearInterval(intervalID8);
          this.floarNumber1 == value;
        }
      }, 1000);
    },
      increaseFloarr1() {
      this.floarNumberr1++;
    },
    increaseFloar1() {
      this.floarNumber1++;
    },
      increaseFloarrs1(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloarr1();
        if (this.floarNumberr1 == value) {
          this.changeColorr11 = value;
          clearInterval(intervalID8);
          this.floarNumberr1 == value;
        }
      }, 1000);
    },
        increaseLift2() {
      this.number2--;
    },
 decreaseFloarrs1(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr1();
        if (this.floarNumberr1 == value) {
          this.changeColorr11 = value;
          clearInterval(intervalID2);
          this.floarNumberr1 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr1 == 0) {
          this.changeColorr11 = 0;
          clearInterval(intervalID2);
          this.floarNumberr1 = "G";
        }
      }, 1000);
    },
       decreaseFloars1(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar1();
        if (this.floarNumber1 == value) {
          this.changeColor11 = value;
          clearInterval(intervalID2);
          this.floarNumber1 = value;

          console.log("Door Open");
        } else if (this.floarNumber1 == 0) {
          this.changeColor11 = 0;
          clearInterval(intervalID2);
          this.floarNumber1 = "G";
        }
      }, 1000);
    },
    decreaseLift2() {
      this.number2++;
    },
    decreaseFloarrs2(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr2();
        if (this.floarNumberr2 == value) {
          this.changeColorr22 = value;
          clearInterval(intervalID2);
          this.floarNumberr2 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr2 == 0) {
          this.changeColorr22 = 0;
          clearInterval(intervalID2);
          this.floarNumberr2 = "G";
        }
      }, 1000);
    },
    goingUp2() {
      this.changeColorD2 = false;
      this.number2 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift2();
        if (this.number2 == 2) {
          clearInterval(intervalID);
          this.changeColorM2 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    goingDown2() {
      this.changeColorM2 = false;
      let intervalID = setInterval(() => {
        this.increaseLift2();
        if (this.number2 === 0) {
          clearInterval(intervalID);
          this.changeColorD2 = true;
          console.log("Interval Cleared");
          this.number2 = "G";
        }
      }, 1000);
    },
    decreaseFloar2() {
      this.floarNumber2--;
    },

    decreaseFloarr2() {
      this.floarNumberr2--;
    },
      increaseFloars2(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloar2();
        if (this.floarNumber2 == value) {
          this.changeColor22 = value;
          clearInterval(intervalID8);
          this.floarNumber2 == value;
        }
      }, 1000);
    },
      increaseFloarr2() {
      this.floarNumberr2++;
    },
    increaseFloar2() {
      this.floarNumber2++;
    },
      increaseFloarrs2(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloarr2();
        if (this.floarNumberr2 == value) {
          this.changeColorr22 = value;
          clearInterval(intervalID8);
          this.floarNumberr2 == value;
        }
      }, 1000);
    },
    decreaseFloarrs2(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr2();
        if (this.floarNumberr2 == value) {
          this.changeColorr22 = value;
          clearInterval(intervalID2);
          this.floarNumberr2 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr2 == 0) {
          this.changeColorr22 = 0;
          clearInterval(intervalID2);
          this.floarNumberr2 = "G";
        }
      }, 1000);
    },
       decreaseFloars2(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar2();
        if (this.floarNumber2 == value) {
          this.changeColor22 = value;
          clearInterval(intervalID2);
          this.floarNumber2 = value;

          console.log("Door Open");
        } else if (this.floarNumber2 == 0) {
          this.changeColor22 = 0;
          clearInterval(intervalID2);
          this.floarNumber2 = "G";
        }
      }, 1000);
    },
        increaseLift3() {
      this.number3--;
    },

    decreaseLift3() {
      this.number3++;
    },
    decreaseFloarrs3(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr3();
        if (this.floarNumberr3 == value) {
          this.changeColorr33 = value;
          clearInterval(intervalID2);
          this.floarNumberr3 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr3 == 0) {
          this.changeColorr33 = 0;
          clearInterval(intervalID2);
          this.floarNumberr3 = "G";
        }
      }, 1000);
    },
    goingUp3() {
      this.changeColorD3 = false;
      this.number3 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift3();
        if (this.number3 == 3) {
          clearInterval(intervalID);
          this.changeColorM3 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    goingDown3() {
      this.changeColorM3 = false;
      let intervalID = setInterval(() => {
        this.increaseLift3();
        if (this.number3 === 0) {
          clearInterval(intervalID);
          this.changeColorD3 = true;
          console.log("Interval Cleared");
          this.number3 = "G";
        }
      }, 1000);
    },
    decreaseFloar3() {
      this.floarNumber3--;
    },

    decreaseFloarr3() {
      this.floarNumberr3--;
    },
     increaseFloars3(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloar3();
        if (this.floarNumber3 == value) {
          this.changeColor33 = value;
          clearInterval(intervalID8);
          this.floarNumber3 == value;
        }
      }, 1000);
    },
      increaseFloarr3() {
      this.floarNumberr3++;
    },
    increaseFloar3() {
      this.floarNumber3++;
    },
      increaseFloarrs3(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloarr3();
        if (this.floarNumberr3 == value) {
          this.changeColorr33 = value;
          clearInterval(intervalID8);
          this.floarNumberr3 == value;
        }
      }, 1000);
    },
     decreaseFloarrs3(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr3();
        if (this.floarNumberr3 == value) {
          this.changeColorr33 = value;
          clearInterval(intervalID2);
          this.floarNumberr3 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr3 == 0) {
          this.changeColorr33 = 0;
          clearInterval(intervalID2);
          this.floarNumberr3 = "G";
        }
      }, 1000);
    },
       decreaseFloars3(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar3();
        if (this.floarNumber3 == value) {
          this.changeColor33 = value;
          clearInterval(intervalID2);
          this.floarNumber3 = value;

          console.log("Door Open");
        } else if (this.floarNumber3 == 0) {
          this.changeColor33 = 0;
          clearInterval(intervalID2);
          this.floarNumber3 = "G";
        }
      }, 1000);
    },
     increaseLift4() {
      this.number4--;
    },

    decreaseLift4() {
      this.number4++;
    },
    decreaseFloarrs4(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr4();
        if (this.floarNumberr4 == value) {
          this.changeColorr44 = value;
          clearInterval(intervalID2);
          this.floarNumberr4 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr4 == 0) {
          this.changeColorr44 = 0;
          clearInterval(intervalID2);
          this.floarNumberr4 = "G";
        }
      }, 1000);
    },
    goingUp4() {
      this.changeColorD4 = false;
      this.number4 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift4();
        if (this.number4 == 4) {
          clearInterval(intervalID);
          this.changeColorM4 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    goingDown4() {
      this.changeColorM4 = false;
      let intervalID = setInterval(() => {
        this.increaseLift4();
        if (this.number4 === 0) {
          clearInterval(intervalID);
          this.changeColorD4 = true;
          console.log("Interval Cleared");
          this.number4 = "G";
        }
      }, 1000);
    },
    decreaseFloar4() {
      this.floarNumber4--;
    },

    decreaseFloarr4() {
      this.floarNumberr4--;
    },
      increaseFloars4(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloar4();
        if (this.floarNumber4 == value) {
          this.changeColor44 = value;
          clearInterval(intervalID8);
          this.floarNumber4 == value;
        }
      }, 1000);
    },
      increaseFloarr4() {
      this.floarNumberr4++;
    },
    increaseFloar4() {
      this.floarNumber4++;
    },
      increaseFloarrs4(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloarr4();
        if (this.floarNumberr4 == value) {
          this.changeColorr44 = value;
          clearInterval(intervalID8);
          this.floarNumberr4 == value;
        }
      }, 1000);
    },
    decreaseFloarrs4(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr4();
        if (this.floarNumberr4 == value) {
          this.changeColorr44 = value;
          clearInterval(intervalID2);
          this.floarNumberr4 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr4 == 0) {
          this.changeColorr44 = 0;
          clearInterval(intervalID2);
          this.floarNumberr4 = "G";
        }
      }, 1000);
    },
       decreaseFloars4(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar4();
        if (this.floarNumber4 == value) {
          this.changeColor44 = value;
          clearInterval(intervalID2);
          this.floarNumber4 = value;

          console.log("Door Open");
        } else if (this.floarNumber4 == 0) {
          this.changeColor44 = 0;
          clearInterval(intervalID2);
          this.floarNumber4 = "G";
        }
      }, 1000);
    },
   increaseLift5() {
      this.number5--;
    },

    decreaseLift5() {
      this.number5++;
    },
    decreaseFloarrs5(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr5();
        if (this.floarNumberr5 == value) {
          this.changeColorr55 = value;
          clearInterval(intervalID2);
          this.floarNumberr5 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr5 == 0) {
          this.changeColorr55 = 0;
          clearInterval(intervalID2);
          this.floarNumberr5 = "G";
        }
      }, 1000);
    },
     increaseFloars5(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloar5();
        if (this.floarNumber5 == value) {
          this.changeColor55 = value;
          clearInterval(intervalID8);
          this.floarNumber5 == value;
        }
      }, 1000);
    },
      increaseFloarr5() {
      this.floarNumberr5++;
    },
    increaseFloar5() {
      this.floarNumber5++;
    },
      increaseFloarrs5(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloarr5();
        if (this.floarNumberr5 == value) {
          this.changeColorr55 = value;
          clearInterval(intervalID8);
          this.floarNumberr5 == value;
        }
      }, 1000);
    },
    goingUp5() {
      this.changeColorD5 = false;
      this.number5 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift5();
        if (this.number5 == 5) {
          clearInterval(intervalID);
          this.changeColorM5 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    goingDown5() {
      this.changeColorM5 = false;
      let intervalID = setInterval(() => {
        this.increaseLift5();
        if (this.number5 === 0) {
          clearInterval(intervalID);
          this.changeColorD5 = true;
          console.log("Interval Cleared");
          this.number5 = "G";
        }
      }, 1000);
    },
      decreaseFloars5(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar5();
        if (this.floarNumber5 == value) {
          this.changeColor55 = value;
          clearInterval(intervalID2);
          this.floarNumber5 = value;

          console.log("Door Open");
        } else if (this.floarNumber5 == 0) {
          this.changeColor55 = 0;
          clearInterval(intervalID2);
          this.floarNumber5 = "G";
        }
      }, 1000);
    },
    decreaseFloar5() {
      this.floarNumber5--;
    },

    decreaseFloarr5() {
      this.floarNumberr5--;
    },
   
    increaseLift6() {
      this.number6--;
    },

    decreaseLift6() {
      this.number6++;
    },
    decreaseFloarrs6(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr6();
        if (this.floarNumberr6 == value) {
          this.changeColorr66 = value;
          clearInterval(intervalID2);
          this.floarNumberr6 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr6 == 0) {
          this.changeColorr66 = 0;
          clearInterval(intervalID2);
          this.floarNumberr6 = "G";
        }
      }, 1000);
    },
    goingUp6() {
      this.changeColorD6 = false;
      this.number6 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift6();
        if (this.number6 == 6) {
          clearInterval(intervalID);
          this.changeColorM6 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    goingDown6() {
      this.changeColorM6 = false;
      let intervalID = setInterval(() => {
        this.increaseLift6();
        if (this.number6 === 0) {
          clearInterval(intervalID);
          this.changeColorD6 = true;
          console.log("Interval Cleared");
          this.number6 = "G";
        }
      }, 1000);
    },
    decreaseFloar6() {
      this.floarNumber6--;
    },

    decreaseFloarr6() {
      this.floarNumberr6--;
    },
      increaseFloarrs6(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloarr6();
        if (this.floarNumberr6 == value) {
          this.changeColorr66 = value;
          clearInterval(intervalID8);
          this.floarNumberr6 == value;
        }
      }, 1000);
    },
    increaseFloar6() {
      this.floarNumber6++;
    },
  
    increaseFloars6(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloar6();
        if (this.floarNumber6 == value) {
          this.changeColor66 = value;
          clearInterval(intervalID8);
          this.floarNumber6 == value;
        }
      }, 1000);
    },
    decreaseFloars6(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar6();
        if (this.floarNumber6 == value) {
          this.changeColor66 = value;
          clearInterval(intervalID2);
          this.floarNumber6 = value;

          console.log("Door Open");
        } else if (this.floarNumber6 == 0) {
          this.changeColor66 = 0;
          clearInterval(intervalID2);
          this.floarNumber6 = "G";
        }
      }, 1000);
    },
    increaseFloarr6() {
      this.floarNumberr6++;
    },
    goingUp7() {
      this.changeColorD7 = false;
      this.number7 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift7();
        if (this.number7 == 7) {
          clearInterval(intervalID);
          this.changeColorM7 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    decreaseLift7() {
      this.number7++;
    },
    increaseLift7() {
      this.number7--;
    },
  
    goingDown7() {
      this.changeColorM7 = false;
      let intervalID = setInterval(() => {
        this.increaseLift7();
        if (this.number7 === 0) {
          clearInterval(intervalID);
          this.changeColorD7 = true;
          console.log("Interval Cleared");
          this.number7 = "G";
        }
      }, 1000);
    },
    decreaseFloar7() {
      this.floarNumber7--;
    },

    decreaseFloarr7() {
      this.floarNumberr7--;
    },
    increaseFloar7() {
      this.floarNumber7++;
    },
    increaseFloars7(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloar7();
        if (this.floarNumber7 == value) {
          this.changeColor77 = value;
          clearInterval(intervalID8);
          this.floarNumber7 == value;
        }
      }, 1000);
    },
    increaseFloarr7() {
      this.floarNumberr7++;
    },
    increaseFloarrs7(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloarr7();
        if (this.floarNumberr7 == value) {
          this.changeColorr77 = value;
          clearInterval(intervalID8);
          this.floarNumberr7 == value;
        }
      }, 1000);
    },
    decreaseFloars7(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar7();
        if (this.floarNumber7 == value) {
          this.changeColor77 = value;
          clearInterval(intervalID2);
          this.floarNumber7 = value;

          console.log("Door Open");
        } else if (this.floarNumber7 == 0) {
          this.changeColor77 = 0;
          clearInterval(intervalID2);
          this.floarNumber7 = "G";
        }
      }, 1000);
    },
    decreaseFloarrs7(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr7();
        if (this.floarNumberr7 == value) {
          this.changeColorr77 = value;
          clearInterval(intervalID2);
          this.floarNumberr7 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr7 == 0) {
          this.changeColorr77 = 0;
          clearInterval(intervalID2);
          this.floarNumberr7 = "G";
        }
      }, 1000);
    },
    goingUp8() {
      this.changeColorD8 = false;
      this.number8 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift2();
        if (this.number8 == 8) {
          clearInterval(intervalID);
          this.changeColorM8 = true;
          // this.number9 = '9'
        }
      }, 1000);
    },
    goingDown8() {
      this.changeColorM8 = false;
      let intervalID = setInterval(() => {
        this.increaseLift2();
        if (this.number8 === 0) {
          clearInterval(intervalID);
          this.changeColorD8 = true;
          console.log("Interval Cleared");
          this.number8 = "G";
        }
      }, 1000);
    },
      increaseFloars8(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloar8();
        if (this.floarNumber8 == value) {
          this.changeColor88 = value;
          clearInterval(intervalID8);
          this.floarNumber8 == value;
        }
      }, 1000);
    },
    increaseLift2() {
      this.number2--;
    },
    decreaseLift2() {
      this.number8++;
    },

    decreaseFloar8() {
      this.floarNumber8--;
    },
    decreaseFloarr8() {
      this.floarNumberr8--;
    },
    increaseFloar8() {
      this.floarNumber8++;
    },

    increaseFloarr8() {
      this.floarNumberr8++;
    },

    increaseFloarrs8(value) {
      let intervalID8 = setInterval(() => {
        this.increaseFloarr8();
        if (this.floarNumberr8 == value) {
          this.changeColorr88 = value;
          clearInterval(intervalID8);
          this.floarNumberr8 == value;
        }
      }, 1000);
    },

    decreaseFloars8(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar8();
        if (this.floarNumber8 == value) {
          this.changeColor88 = value;
          clearInterval(intervalID2);
          this.floarNumber8 = value;

          console.log("Door Open");
        } else if (this.floarNumber8 == 0) {
          this.changeColor88 = 0;
          clearInterval(intervalID2);
          this.floarNumber8 = "G";
        }
      }, 1000);
    },

    decreaseFloarrs8(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr8();
        if (this.floarNumberr8 == value) {
          this.changeColorr88 = value;
          clearInterval(intervalID2);
          this.floarNumberr8 = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr8 == 0) {
          this.changeColorr88 = 0;
          clearInterval(intervalID2);
          this.floarNumberr8 = "G";
        }
      }, 1000);
    },

    goingUp() {
      this.changeColorD = false;
      this.number9 = 1;
      let intervalID = setInterval(() => {
        this.decreaseLift1();
        if (this.number9 == 9) {
          clearInterval(intervalID);
          this.changeColorM = true;
          // this.number9 = '9'
        }
      }, 1000);
    },

    goingDown() {
      this.changeColorM = false;
      let intervalID = setInterval(() => {
        this.increaseLift1();
        if (this.number9 === 0) {
          clearInterval(intervalID);
          this.changeColorD = true;
          console.log("Interval Cleared");
          this.number9 = "G";
        }
      }, 1000);
    },
    increaseLift1() {
      this.number1--;
    },
    decreaseLift1() {
      this.number9++;
    },

    decreaseFloar9() {
      this.floarNumber--;
    },

    decreaseFloarr9() {
      this.floarNumberr--;
    },

    decreaseFloar(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloar9();
        if (this.floarNumber == value) {
          this.changeColor = value;
          clearInterval(intervalID2);
          this.floarNumber = value;

          console.log("Door Open");
        } else if (this.floarNumber == 0) {
          this.changeColor = 0;
          clearInterval(intervalID2);
          this.floarNumber = "G";
        }
      }, 1000);
    },
    decreaseFloarr(value) {
      let intervalID2 = setInterval(() => {
        this.decreaseFloarr9();
        if (this.floarNumberr == value) {
          this.changeColorr = value;
          clearInterval(intervalID2);
          this.floarNumberr = value;

          console.log("Door Open", this.changeColor);
        } else if (this.floarNumberr == 0) {
          this.changeColorr = 0;
          clearInterval(intervalID2);
          this.floarNumberr = "G";
        }
      }, 1000);
    },
  },
};
</script>

<style>
</style>