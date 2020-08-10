<template>
    <div>
        <div>
            Hello this is vue app with vue-cli
        </div>

        <div>
            Let's play with mention animal do you like
        </div>

        <div>
            <h3>
                animal
            </h3>
            <ul>
                <li v-for="(animal, index) in animals " :key="index">
                    {{animal.type}} - {{animal.name}} ({{animal.age}})
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            animals: [
                {
                    type: 'cat',
                    name: 'tom',
                    age: 4,
                },
                {
                    type: 'dog',
                    name: 'bark',
                    age: 5,
                }
            ]
        }
    }

}
</script>