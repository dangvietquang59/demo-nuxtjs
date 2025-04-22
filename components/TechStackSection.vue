<template>
    <div class="min-h-[700px] flex flex-col gap-[20px]">
        <BaseBadge>Techologies Stack</BaseBadge>

        <div class="grid grid-cols-4 gap-[20px]">
            <div
                class="w-[200px] h-[200px] rounded-full overflow-hidden flex items-center justify-center"
            >
                <NuxtImg
                    src="https://i0.wp.com/i.postimg.cc/bJHg5q0K/ReactJS.jpg?w=1300&ssl=1"
                    alt="react"
                />
            </div>
        </div>
    </div>
</template>

<script>
    const routes = [{ name: 'ReactJS', imageUrl: '/' }]
</script>
