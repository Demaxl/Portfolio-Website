<template>
    <div class="my-10 lg:!my-[80px]">
        <h1 class="section-heading"><span>My</span><span>Testimonial</span></h1>

        <div
            class="flex flex-col space-y-10 md:flex-row md:justify-center md:space-x-8 md:space-y-0"
        >
            <template v-for="(testimonial, index) in testimonials" :key="index">
                <TestimonialCard v-bind="testimonial" :index="index" />
            </template>
        </div>
    </div>
</template>

<script setup>
import TestimonialCard from '@/components/TestimonialCard.vue'

const testimonials = [
    {
        name: 'Evran Shah',
        position: 'Designer',
        testimonial:
            'I recently had to jump on 10+ different calls across eight different countries to find the right owner.',
        gender: 'male',
        link: 'https://www.example.com'
    },
    {
        name: 'Flora Sheen',
        position: 'Designer',
        testimonial:
            'I recently had to jump on 10+ different calls across eight different countries to find the right owner.',
        gender: 'female',
        link: 'https://www.example.com'
    },
    {
        name: 'Evran Shah',
        position: 'Designer',
        testimonial:
            'I recently had to jump on 10+ different calls across eight different countries to find the right owner.',
        gender: 'male',
        link: 'https://www.example.com'
    }
]
</script>
